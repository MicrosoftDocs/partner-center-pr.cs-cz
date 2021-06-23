---
title: Migrace z programu Partner Sales Connect (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak mohou partneři Microsoftu migrovat ze služby Partner Sales Connect (PSC) Partnerské centrum a vytvářet a spravovat dohody odeslané prodejci Microsoftu.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 5be1c09a26cfcc0d038663e5814ccda7e535d4d1
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551431"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Průvodce spoluprodejem v partnerském Partnerské centrum (PC) pro partnery migrující z programu Partner Sales Connect (PSC)

**Odpovídající role:** Správce účtu | Referenční | Partner Sales Connect (PSC) seller | Partner Sales Connect (PSC) admin | Partner Sales Connect (PSC) Deal Manager

Tento článek obsahuje pokyny pro partnery migrující z Partner Sales Connect (PSC) na Partnerské centrum (PC), aby mohli pokračovat ve vytváření a správě dohod o spoluprodeji v Partnerské centrum.

>[!Note]
> Pokud jste tady, protože jste v PSC viděli banner o migraci, jste na správném místě. Tato příručka není platná pro obchodní partnery pro licencování OEM a posouzení řešení (SA) a OEM, kteří spravují své obchody v PSC.

>[!Important]
> Od 1. dubna 2021 vaše společnost nebude moct v PSC vytvářet ani upravovat dohody. **Pomocí funkce hromadného exportu v PSC si stále budete moct stáhnout existující data o obchodech. Otevřené obchody [můžete také migrovat](psc-to-pc.md#psc-deals-migration) z PSC do Partnerské centrum po tomto datu.** <br><br> Pokud aktivně pracujete na dohodám, které obsahují řešení s nárokem na pobídky v rámci spoluproduování IP adres, máte dvě možnosti: <br><br> 1. Před 31. březnem 2021 označte dohodu jako won a dokončete registraci dohody v PSC. <br> 2. [Migrace dohod na](psc-to-pc.md#psc-deals-migration) Partnerské centrum abyste měli více času na práci na dohody a zahájení registrace dohody.

Jak víte, **firma ztratí přístup k PSC po 30. dubnu 2021.** Stále ale najdete všechno, co chcete dělat v Partnerské centrum, jako je vytváření dohod o spoluprodávači, správa dohod a akce, které vám poslali prodejci Microsoftu.

Budou ale mezi nimi rozdíly. Následující pokyny vám můžou pomoct zajistit, aby byl přechod Partnerské centrum plynulejší a jednodušší.

## <a name="before-you-move-things-you-need-to-know"></a>Co potřebujete vědět, než se přesunete

### <a name="if-you-are-a-psc-admin"></a>Pokud jste správcem PSC

- Pracovní e-mail potřebujete pro přihlášení k [Partnerské centrum](https://partner.microsoft.com/).
- Nastavte svůj účet pomocí správce Partnerské centrum [účtu.](permissions-overview.md)
- Přečtěte si tento dokument a zjistěte, jak Partnerské centrum spoluprodávat v tomto dokumentu.
- Nastavte uživatelské účty v Partnerské centrum pro všechny uživatele PSC (role správce, správce dohody a prodejce) a přiřaďte jim role [správce referenčních seznamu.](permissions-overview.md)

>[!IMPORTANT]
> Zkontrolujte, že ID Microsoft Partner Network (MPN) zobrazené v banneru PSC je k dispozici v seznamu umístění MPN v Partnerské centrum.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Obrázek znázorňující banner PSC, kde partneři mohou najít ID MPN":::

 Pokud chcete ověřit, že se ID MPN zobrazuje jako umístění MPN Partnerské centrum, přihlaste se k řídicímu panelu [Partnerské centrum,](https://partner.microsoft.com/dashboard)pak v pravém horním rohu obrazovky vyberte Nastavení **(ikona** ozubeného kola) a pak Nastavení **účtu.** V levé navigační nabídce druhé úrovně  vyberte Umístění. Zobrazí se seznam všech ID a umístění MPN přidružených k účtu mpn Partnerské centrum účtu.

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

1. Vyberte **Nastavení účtu** z ikony ozubeného kola v pravém horním rohu řídicího Partnerské centrum zařízení.

1. V **levé navigační** nabídce druhé úrovně vyberte Správa uživatelů.

1. V horní části seznamu uživatelů vyberte **rozevírací** nabídku Filtr. Změňte možnost na **Správce účtu.**

   Na stránce se zobrazí všichni správci účtu s příslušnými e-mailových adresami. Jednomu z nich pošlete e-mail a požádejte ho, aby přiřadili roli správce referenčních seznamu pro váš pracovní účet.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="Obrázek znázorňující správce účtu na stránce pro správu uživatelů v nastavení partnera":::

>[!Important]
>- Pokud vaše role zahrnuje jenom správu uživatelů v PSC, požádejte [](permissions-overview.md#manage-mpn-membership-and-your-company) správce účtu vaší společnosti, aby vám přiřadí roli správce účtu v Partnerské centrum. 
>- Pokud vaše role také zahrnuje správu příležitostí ke spoluprodání, požádejte o přiřazení role [správce referenčních](permissions-overview.md#manage-referrals) odkazů.
> - Je vhodné také nominovat jednoho vedoucího řízení změn mezi správci PSC. Tím zabráníte tomu, aby se všichni správci PSC museli jednotlivě kontaktovat Partnerské centrum účtu. Místo toho může být vedoucí správy změn primární osobou, která pracuje s Partnerské centrum účtem.

## <a name="user-migration"></a>Migrace uživatelů

Po nastavení účtu v Partnerské centrum můžete pomocí průvodce migrací uživatelů na stránce Příležitosti ke spoluprodávu automaticky přiřazovat Partnerské centrum role zaměstnancům vaší společnosti.

>[!Note]
> Migraci uživatelů mohou provádět pouze [správci](permissions-overview.md#manage-mpn-membership-and-your-company) účtů vaší společnosti. Pokud nemáte roli správce účtu, najděte správce účtu, který vám může pomoct nastavit uživatelské účty pomocí průvodce migrací uživatelů.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Obrázek znázorňující průvodce migrací uživatelů":::

Správcům účtu se na stránce příležitosti ke spoluprodávce vedle referenčních odkazů zobrazí odkaz průvodce migrací uživatelů DOS. Výběrem odkazu mohou zahájit migraci uživatelů. Pokud chcete zahájit migraci uživatelů, mohou správci tento odkaz vybrat. Tento krok migrace uživatelů může provést vícekrát, dokud nebudou mít všichni uživatelé přiřazené správné role v Partnerské centrum.

Tabulka migrace uživatelů obsahuje následující podrobnosti:

- Uživatelský účet – ID e-mailu zaměstnance
- Partnerský účet PSC – Účet, ke kterému je zaměstnanec přidružený v PSC
- Role uživatele PSC – jedna ze tří rolí přiřazených v PSC.
- Umístění PC MPN – umístění, pro které bude mít uživatel příslušné Partnerské centrum (PC). MPN partnerského účtu PSC slouží k vyhledání ekvivalentního umístění MPN v Partnerské centrum přiřazení oprávnění. Celá organizace označuje ID MPN vOrg.
- Role uživatele počítače – Zaměstnanci mají přiřazené role na základě jejich uživatelských rolí PSC. Správce v PSC bude mít přiřazené role správce referenčních Partnerské centrum. Prodejce bude mít přiřazenou roli uživatele referenčních Partnerské centrum. Další informace o rolích Partnerské centrum a o tom, co uživatelé s těmito rolemi mohou dělat v [Partnerské centrum.](permissions-overview.md#manage-referrals)
- Pc AAD Tenant – tenant Microsoft Azure Active Directory (Azure AD), ke kterému jsou uživatelé přiřazení v Partnerské centrum
- Stav – Existují tři možné stavy pro stav migrace.
    - **Nemigrován** – Uživatel nemá přiřazenou žádnou Partnerské centrum referenčních odkazů.
    - **Migrován** – Uživatel byl úspěšně migrován s přiřazenou odpovídající rolí, jak je znázorněno v tabulce.
    - **Chyba** – Migraci se nepodařilo dokončit kvůli nějaké chybě

Někdy může migrace selhat a vést k chybám. Tady je několik důvodů, proč migrace může způsobit chybu, a některé způsoby, jak tento problém vyřešit:

1. Uživatelé PSC mohou používat nepracují účet.

2. Uživatel PSC může používat účet z jiné domény, než kterou používáte v Partnerské centrum.

   Pokud chcete vyřešit chyby související se scénáři 1 a 2, požádejte uživatele, aby se Partnerské centrum pomocí svého pracovního účtu připojeného k vašemu tenantovi Azure AD. Může [vám pomoct globální](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) správce.
   
   Vyhledání globálního správce: 
   - Přihlaste se k Partnerské centrum [a](https://partner.microsoft.com/dashboard) **v** pravém horním rohu vyberte Nastavení účtu z ikony ozubeného kola.
   - Na **levém navigačním** panelu druhé úrovně vyberte Správa uživatelů.
   - V horní části seznamu uživatelů  vyberte rozevírací nabídku Filtr a změňte možnost na **Globální správce.** Na stránce se pak zobrazí všichni globální správci s příslušnými e-mailových adresami. Požádejte jednoho z nich o přiřazení role správce referenčních seznamu pro váš pracovní účet.
   
      Globální správce může buď vytvořit nový uživatelský účet ve vašem tenantovi Azure AD, nebo přiřadit přístup uživatele hosta ostatním uživatelům účtu domény. Jakmile jsou účty nastavené pro všechny správce dohody a uživatele PSC, musí se přihlásit  k Partnerské centrum, v levé navigační nabídce vybrat Referenční odkazy a ověřit, že se jim zobrazí stránka Referenční odkazy.

3. Uživatel už má v seznamu přiřazenou roli Partnerské centrum.
    - Můžete ověřit existující roli uživatele. V pravém horním rohu okna vyberte Partnerské centrum **(ikona** ozubeného kola) a pak **Nastavení účtu.** Když se zobrazí druhá levá navigační nabídka, vyberte **Správa uživatelů** a vyhledejte uživatele.

## <a name="psc-deals-migration"></a>Migrace dohody o PSC

Po dokončení migrace uživatelů použijte průvodce migrací dohody na stránce Příležitosti ke spoluprodávce a přenesete všechny oprávněné otevřené obchody z PSC na Partnerské centrum. **Odkaz na migraci dohody bude viditelný jenom správcům referenčních doporučení s celým rozsahem organizace v Partnerské centrum.** Vpravo nahoře na stránce Příležitosti ke spoluprodávce bude odkaz s názvem Migrace dohody **PSC,** který otevře průvodce migrací dohody.

Před zahájením migrace dohody si přečtěte tuto část.

**Nárok na migraci**

K migraci z PSC na Partnerské centrum. Tento průvodce migrací je vytvořen tak, aby partnerům pomohl Partnerské centrum, kde stále aktivně spolupracuje se svými zákazníky na uzavření dohody. **Na migraci mají nárok jenom dohody, které jsou v otevřeném stavu vytvořené od 1. ledna 2020 s platnými podrobnostmi o partnerském účtu (platné ID MPN) a procházejí registrací dohody.**

**Není možné migrací**

- Dohody o posouzení řešení nemají nárok na migraci dohody
- Obchodní dohody o licencování OEM nemají nárok na migraci dohody
- Žádná dohoda, která byla v PSC označena jako vyhrála, nemá nárok na migraci. Registrace dohody, pokud má nárok na obchody označené jako won, by se měla dokončit v PSC.

## <a name="pre-requisites-for-deal-migration"></a>Předpoklady pro migraci dohody

Před zahájením migrace dohody z Partnerské centrum podle následujících pokynů nastavte obchody v PSC pro úspěšnou migraci.

1. O této migraci jsou informováni všichni členové prodejního týmu ve vaší společnosti, kteří pracují na otevřených obchodech.
2. Členové prodejního týmu jsou vytrénované tak, aby Partnerské centrum k řízení dohody.
3. Obchody mají všechny požadované informace, jak je popsáno níže.
    - Podrobnosti o společnosti zákazníka včetně názvu a adresy
    - Kontaktní údaje zákazníka, pokud se jedná o dohodu o spoluprodát
    - Alespoň jedno řešení
    - Alespoň jeden člen týmu se všemi podrobnostmi – jméno, příjmení, ID e-mailu a telefonní číslo
    - Hodnota dohody
    - Odhadované datum uzavření dohody
    - Poznámky pro partnery

Pomocí možností hromadného stahování a nahrávání v PSC můžete přidat všechny chybějící podrobnosti v rámci dohody pro všechny oprávněné dohody.

>[!Note]
> Migrace dohody bude úspěšná i v případě, že výše uvedené požadavky nebudou splněny. Nemůžete ale změnit stav dohody, pokud některé z výše uvedených požadovaných polí v Partnerské centrum nejsou k dispozici. Pak budete muset zadat všechny požadované informace, které v obchodech chybí Partnerské centrum na nich začít pracovat. **Před migrací oprávněných obchodů v PSC důrazně doporučujeme vyčistit je Partnerské centrum.**

Migrace dohody v Partnerské centrum je sestavená jako prostředí jedním kliknutím. Jakmile bude vaše společnost  připravená na migraci oprávněných dohod, musíte vybrat tlačítko Migrovat obchody. **Nemůžete zvolit dohody, které chcete migrovat z PSC. Pokud nechcete migrovat žádné dohody do Partnerské centrum, před zahájením migrace je přesuňte do uzavřeného stavu v PSC.**

>[!Note]
> Po zahájení migrace může migrace dohod trvat až **24 hodin.**

Po dokončení migrace se stav banneru změní tak, aby se dokončil s odkazem na sestavu migrace. Stáhněte si sestavu, abyste si prohlédněte podrobnosti o dohodách, které se migrují z PSC do Partnerské centrum.

Sestava obsahuje následující podrobnosti.

1. **Partnerské centrum zapojení –** jedinečný identifikátor v Partnerské centrum pro všechny obchody v rámci zapojení. Existují dvě dohody – jedna pro partnera a jedna pro Microsoft ve spolupráci v Partnerské centrum.
2. **Partnerské centrum referenčního odkazu** – jedinečný identifikátor Partnerské centrum pro dohodu, která patří partnerovi.
3. **Název dohody** – identifikátor zadaný pro dohodu v PSC.
4. **ID dohody PSC** – jedinečný identifikátor v PSC pro dohodu.
5. **Chyby** – značí, jestli při migraci konkrétní dohody dojde k nějaké chybě.

Všechny obchody, které byly úspěšně migrovány, se v PSC nezobrazí. Migrované dohody můžete dál pracovat v Partnerské centrum včetně dokončení registrace dohody v Partnerské centrum. Interakce s prodejci Microsoftu při dohodách o spoluprodávačích se nemění.

Dohody migrované z PSC budou k dispozici na kartách Příchozí a Odchozí v závislosti na zdroji dohody. Všechny dohody sdílené vaší společností budou dostupné na kartě Odchozí a dohody iniciované Microsoftem budou k dispozici na kartě Příchozí v Partnerské centrum. Po migraci budou vytvořeny dva typy dohod.

1. **Dohody o spoluprodávce** – Dohody, které jsou v PSC označené jako spoluprodávné, se vytvoří jako dohody o spoluprodávce v Partnerské centrum.
2. **Dohody vedené partnery** – Dohody, které nejsou označené jako spoluprodáky, se vytvoří jako dohody vedené partnery v Partnerské centrum. Dohody vedené partnery jsou viditelné prodejcům Microsoftu a před dosažením terminálových stavů (won, lost) je možné upgradovat na dohody o spoluprodávači. Dohody vedené partnery mají také nárok na registraci dohody, pokud se v rámci dohody nachází řešení s nárokem na pobídky.

>[!Important]
> Pokud dojde k chybám, kvůli kterým se některé dohody nemigrují, můžete migraci dohody znovu zahájit kliknutím na tlačítko **Migrovat dohody.** Tato možnost se povolí jenom v případě, že ještě existuje několik oprávněných dohod, které se mají migrovat. To bude užitečné také v případě, že jste ve fázi přechodu, ve které se v PSC vytvářejí nové dohody po zahájení migrace dohody.

Po úspěšné migraci všech dohod se zobrazí banner No **deals to migrate** (Žádné dohody o migraci) se zakázaným tlačítkem Migrate **deals** (Migrace **dohod).**

Po dokončení migrace uživatelů nebo dohody o migraci použijte následující pokyny k rozhodnutí o strategii migrace:

Pokud má vaše společnost manažera pro vývoj partnerů (PDM) – Když je váš účet Partnerské centrum nastavený a vaši uživatelé se přesunuli a mají role a oprávnění, můžete aktivity spoluprodáva přesunout do Partnerské centrum. Informujte pdm, aby přepne, místo abyste čekali na dokončení migrace, což umožní, aby se všechny nové obchody dostaly do Partnerské centrum.

>[!Note]
>Jakmile tento přepínač změníte, budete moct jednat pouze s existujícími aktivními obchody v PSC. V PSC nemůžete vytvářet nové dohody ani přijímat žádné dohody od prodejců Microsoftu.

Pokud vaše společnost nemá pdm , ujistěte se, že jsou všechny uživatelské účty nastavené a ověřené všemi uživateli. Prostřednictvím e-mailu a banneru v PSC budete upozorněni na přesné datum zahájení spoluprodávek v Partnerské centrum. Mějte na paměti, že stávající aktivní obchody budete muset spravovat i nadále v PSC.

>[!Important]
> Do 30. dubna 2021 máte zaregistrovat obchody označené jako won.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Další kroky pro správce PSC, manažery dohody PSC a prodejce PSC

Naučte se spoluprodávat v Partnerské centrum.
Jedná se o důležitý krok, který vám pomůže být připraveni na spoluprodáva v Partnerské centrum. Porozuměli jste pracovním postupům a změnám v Partnerské centrum, abyste mohli efektivně ihned spoluprodávat. Začněte tím, že si tento dokument kompletně pročtete. Dobrá sada prostředků je k dispozici také v galerii [prostředí spoluprodáce.](https://aka.ms/cosellexperience)

## <a name="major-differences-between-psc-and-partner-center-workflows"></a>Hlavní rozdíly mezi pracovními postupy PSC a Partnerské centrum pracovními postupy

|**Scénář**|**Partner Sales Connect**|**Partnerské centrum**|
|-----|:-----|:-----|
|Role uživatelů|PSC má role správce, manažera dohody a prodejce.|Partnerské centrum má jenom roli [správce referenčních](permissions-overview.md#manage-referrals) seznamu, která uděluje oprávnění ke čtení i zápisu pro všechny obchody.|
|Pozvání Microsoftu k dohody o spoluprodávaní|Inicioval/a prodejce Microsoftu a partner se na to výslovně neptal.|Partner bude muset provést explicitní [žádost, pokud](manage-co-sell-opportunities.md#add-solutions) je pro dohodu potřeba pomoc s prodejcem Microsoftu. Prodejce Microsoftu má možnost žádost odmítnout.|
|Vypršení platnosti|Neexistuje žádný koncept vypršení platnosti dohody.|Platnost příchozích dohod partnerů vyprší za 14 dnů, pokud je partner nepřijme. Totéž platí i pro odchozí dohody partnerů, jejichž platnost vypršela, pokud prodejce Microsoftu za 14 dnů nevyhodí.|
|Podrobnosti o prodejci Microsoftu|Viditelné, jakmile se vytvoří dohoda.|Podrobnosti o prodejci Microsoftu se s partnerem sdílí jenom v případě, že prodejce výslovně přijme pozvánku ke spoluprodávači od partnera.|
|[Privátní kanál](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Není k dispozici.|Partneři mohou sdílet svůj kanál, aniž by prodejci Microsoftu dáváme přehled.|
|Řešení|Řešení, která patří jenom do jednoho ceníku, je možné přidat do dohody.|Partner může přidat [řešení,](manage-co-sell-opportunities.md#add-solutions) která patří do následujících seznamů. a) Vlastní řešení b) Řešení z katalogu Microsoftu první strany (podobně jako u role dohody o transakcích v PSC) a c) Řešení spoluproduování od jiných partnerů třetích stran (podobně jako u role dohody ISV v PSC).|
|Přiřazení dohody|Jen přiřazený prodejce může obchody zobrazit a jednat s ohledem na to.|Členy týmu je možné přidat do dohody, aby mohli určit lidi, kteří pracují na dohody, a ostatní správci referenčních seznamu nemají žádné blokování v zobrazení těchto dohod nebo v jejich náplní.|
|Organizace zákazníků|Zadání textu volného formuláře.|Zadáním několika [znaků můžete v](manage-co-sell-opportunities.md#select-your-customer) organizaci zákazníka vyhledat databázi [D&B.](https://www.dnb.com/) Právní název a adresa se vyplní automaticky podle volby.|
|Kontakt zákazníka|Není povinné.|Pro sdílení privátních kanálů to není povinné. Požadováno v případě, že se prodejce Microsoftu pozve k účasti na žádosti o společný prodej.|
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

Porovnejte párové a očíslované kružnice mezi horním snímkem PSC a snímkem partnerského centra pod ním. Čísla odpovídajících čísel ukazují, kde můžete najít funkci nebo atribut související s PSC v partnerském centru. Červené kroužky označují, že neexistuje žádné odpovídajícího pole partnerského centra.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Obrázek znázorňující mapování polí mezi domovskou stránkou partnera Sales Connect a výchozím zobrazením příležitostí v partnerském centru pro společné prodeje." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 – zobrazení tabulky PSC mapované na zobrazení obchodu v partnerském centru

Porovnejte párové a očíslované kružnice mezi horním snímkem PSC a snímkem partnerského centra pod ním. Čísla odpovídajících čísel ukazují, kde můžete najít funkci nebo atribut související s PSC v partnerském centru. Červené kroužky označují, že neexistuje žádné odpovídajícího pole partnerského centra.  

> [!NOTE]
> Pod snímky obrazovky se zobrazí další požadavky.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Obrázek znázorňující mapování polí mezi zobrazením mřížky partnera Sales Connect (PSC) a zobrazením obchodu v partnerském centru." lightbox="images/pscmigration/grid-view-expanded.png":::

**Zvláštní požadavky:**

- V partnerském centru neexistuje žádné zobrazení seznamu, jako je třeba PBV.  Všechny obchody jsou uvedené na základě nejnovějšího data přijetí nebo vytvoření s informacemi o zákaznících a typu obchodu. Ve výchozím nastavení je vybrán první obchod v zobrazení. Většina hodnot zobrazených ve formátu tabulky PSC je k dispozici v podrobném zobrazení obchodu v partnerském centru.
- Role koupě není požadované pole v partnerském centru. Nezobrazuje se ani se nezachycuje v žádném z pracovních postupů. Je odvozená automaticky na straně prodejce Microsoftu na základě řešení přidaných do obchodu.
- Datum poslední změny se nezobrazí na stránce podrobností odkazu v partnerském centru. Partneři mohou pomocí funkce řazení seřadit obchody na základě data poslední aktualizace.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 – zobrazení podrobností o koupi PSC mapované na partnerské Centrum

Porovnejte párové kroužky na horním (PBV) snímku obrazovky, na které se nachází snímek obrazovky partnerského centra. Čísla odpovídajících čísel ukazují, kde můžete najít funkci nebo atribut související s PSC v partnerském centru. Červené kroužky označují, že v partnerském centru neexistuje žádné vyhovující pole ani oblast.

> [!NOTE]
> Pod snímky obrazovky se zobrazí další požadavky.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Obrázek znázorňující mapování polí mezi zobrazením podrobností o prodeji partnera Sales Connect (PSC) a zobrazení podrobností pro partnerské Centrum" lightbox="images/pscmigration/deal-details-expanded.png":::

**Zvláštní požadavky:**

- Partneři můžou upravit práci výběrem tlačítka upravit v zobrazení podrobností o partnerském obchodu (6). Po výběru tlačítka pro úpravy se všechna pole stanou upravitelná. Pak máte možnost buď uložit, nebo zrušit úpravy provedené v obchodu.
- Neexistuje možnost uzavřít obchod jako duplicitní v partnerském centru.
- Výsledek zákazníka není v partnerském centru k dispozici. Všechny podrobnosti související se zákaznickými interakcemi se dají aktualizovat v části poznámky v partnerském centru.
- Odhadované datum ukončení řešení je k dispozici pouze pro obchody OEM IOT v partnerském centru. Tyto informace se nezobrazují pro žádné jiné typy obchodování.
- Licenční program není vyžadován v partnerském centru. Tyto informace jsou automaticky odvozené v závislosti na řešeních vybraných v obchodu.

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

K tomu dochází pouze v případě, že k organizaci MPN, kterou používáte v rámci programu , nejsou připojená žádná řešení připravená ke spoluprodávce Partnerské centrum. Kontaktujte primární řadič domény a získejte ID MPN vašich řešení opravené nebo vytvořte lístek podpory s informací o problému " Po migraci PSC je tlačítko Nové dohody zašedé".

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 – Můžu přiřadit dohody konkrétní osobě z naší organizace, jako je PSC?

Ke konkrétní dohodu můžete přiřadit členy týmu. Nezablokuje ostatním správcům referenčních nabídek jejich zobrazení ani akce s těmito obchody.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 – Je k dispozici zobrazení všech dohod, které jsou mi přiřazeny?

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

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 – Je přidání zákaznické organizace povinné?

Ano, přidání [organizace zákazníka je](./manage-co-sell-opportunities.md#select-your-customer) ve Partnerské centrum. Nejprve začněte vyhledáním místa, kde se nachází zákazník. Na základě podrobností, které máte. Můžete být konkrétní, včetně přesného názvu budovy, nebo prostě dejte podrobnosti o městě. Vyhledávání v organizaci načte všechny právní entity odpovídající názvu, který zadáte, takže nemusíte zadávat žádné podrobnosti o adrese. Všechny podrobnosti se vyplní automaticky na základě vybrané organizace.

### <a name="10---are-customer-contact-details-mandatory"></a>10 – Jsou kontaktní údaje zákazníků povinné?

Závisí na [typu dohody, kterou](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) vytváříte. Pokud kanál jenom sdílíte a nevyžadujete žádnou pomoc od prodejní organizace Microsoftu, můžete se rozhodnout neposíolit kontaktní údaje zákazníků. Pokud spoluprodáte, kde aktivně hledáte pomoc od prodejce Microsoftu, budete muset zadat kontaktní údaje zákazníka. Před vytvořením žádosti o spoluprodát v Partnerském centru byste měli od zákazníka získat explicitní souhlas.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 – Kolik řešení můžu přidat do dohody?

Do dohody můžete přidat až 50 řešení (podobně jako u produktů v PSC). Na rozdíl od PSC můžete kombinovat řešení z vlastních oprávněných řešení pro spoluprodávku, skladových náklady Microsoftu a dalších oprávněných řešení pro spoluprodávku třetích stran. V Partnerském centru není vybraná nebo dostupná žádná role dohody. Pro skladové položky Microsoftu můžete volitelně přidat množství a cenu pro každou SKU, která se přidá do dohody.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 – Kdy se po vytvoření dohody se budu seznamovat s podrobnostmi o prodejci Microsoftu?

Prodejci Microsoftu se přiřadí až po vyhotovění přesně uvedeného požadavku na pomoc při vytváření dohody s příslušnou osobou prodejce na straně Microsoftu. I po přiřazení budou mít prodejci Microsoftu možnost pozvánku ke spoluprodávači přijmout nebo odmítnout. Jenom v případě, že prodejce přijme pozvánku ke spoluprodávači, aktualizuje se dohoda s kontaktními údaji na prodejce Microsoftu. Smlouva SLA pro prodejce Microsoftu, kteří se dohodu dohodí, je 14 dnů. Jedná se o stejnou smlouvu SLA, kterou partneři musí na základě dohody jednat, než přejde do stavu, kdy vypršela její platnost.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 – Kde najdu ID příležitosti?

ID příležitosti v PSC je stejné jako ID dohody v Partnerské centrum. ID dohody najdete při otevření dohody vedle názvu dohody.

### <a name="14---how-can-my-pdm-get-access-to-partner-center"></a>14. Jak můj pdm může získat přístup k Partnerské centrum?

Partnerské centrum na rozdíl od PSC k primárním řadičům domény přístup nesdílí. Tuto funkci můžete povolit několika možnostmi, které jsou uvedené níže.

- Přehledy OCP – Pokud si primární počítače jen prohlíhá obchody a průběh, které s nimi souvisejí, mohou k zobrazení vaší organizace použít portál Přehledy OCP (One Commercial Partner). Jedná se o interní nástroj, který je k dispozici pouze pro pdmy. Přehledy OCP nejsou k dispozici pro uživatele vaší společnosti.
- Uživatel hosta v Partnerské centrum – V Partnerském centru můžete přidat svůj účet PDM jako uživatele hosta a přiřadit mu roli správce referenčních seznamu, aby si mohli zobrazit referenční odkazy a úlohu @microsoft.com s nimi stoupit.
- Vytvoření nového uživatele ve vašem tenantovi – Můžete vytvořit nového uživatele ve vlastním tenantovi [a](./create-user-accounts-and-set-permissions.md#add-a-new-user) tyto podrobnosti sdílet s PDM, aby mohl zobrazit referenční seznam podobný ostatním uživatelům referenčních seznamu ve vašem účtu a jednat s ním.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Vyhledání správného ID MPN, pokud váš účet v PSC není přidružený k platnému MPN

Pokud jste tady, protože jste v PSC viděli banner se zmínkou o problému s neplatným přidružením ID MPN v PSC, jste na správném místě. Váš účet mohl být propojený s neplatným ID MPN z následujících důvodů:

- Vaše společnost nemá Partnerské centrum účet.
- Váš PDM udělal chybu při zadávání ID MPN vašeho účtu v interních systémech, které propojují váš účet PSC s vaším Partnerské centrum účtem (ID MPN).
- Vaše společnost migraci z Partner Membership Center (PMC) do Partnerské centrum.

Nejprve pomocí následujících kroků vyhledejte správné ID MPN.

- Přihlaste se ke svému Partnerské centrum účtu.
- K vyhledání ID MPN použijte [pokyny](./partner-center-account-setup.md#locate-your-mpn-id) uvedené v dokumentaci k nastavení účtu.

Níže je snímek obrazovky s přesným umístěním, kde najdete Partnerské centrum MPN.

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="Obrázek znázorňující nastavení účtu, kde partner může najít své ID MPN"  lightbox="images/pscmigration/findingMPNID.png":::

Další, 

- Pokud máte pdm, požádejte ho, aby vaše ID MPN opravili pomocí správného ID MPN z vašeho účtu v Partnerském centru.
- Pokud nemáte pdm, odešlete e-mail na adresu v banneru PSC s informacemi o účtu PSC zobrazenými v banneru PSC a správným ID MPN z vašeho účtu v Partnerském centru.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Zdroje informací, které vám pomůžou vytvářet a spravovat obchody v Partnerské centrum

Pokud jste si ještě nečetl témata nápovědy ke spoluprodátu, následující zdroje informací vám pomůžou se spravovat obchody v Partnerském centru.

|**Chcete-li to provést**   |**Přečtěte si:**   |
|-----------------------|:-----------------------|
|Vysvětlení karet a navigace na stránce příležitosti ke spoluprodání|[Navigace v oddílu spoluprodádání](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Výběr organizace zákazníka ze seznamu D&B |[Výběr zákazníka](./manage-co-sell-opportunities.md#select-your-customer)|
|Úprava polí v části podrobnosti dohody|[Podrobnosti o dohody](./manage-co-sell-opportunities.md#deal-details)|
|Přidání členů týmu do dohody|[Přidání zaměstnanců](./manage-co-sell-opportunities.md#add-team-members)|
|Reakce na dohodu o spoluprodátu|[Správa dohod o spoluprodátu](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Registrace dohod, které jste vyhráli v Partnerské centrum |[Registrace nové dohody](./register-deals.md)
|Získejte přehledy referenčních seznamu a zjistěte, jak si vaše referenční reference vede. |[Přehledy referenčních seznamů](./referral-insights.md)
|Vytvoření a správa obchodního profilu|[Správa obchodního profilu](./create-a-marketing-profile.md)
|Správa potenciálních zákazníků pro obchodní profil |[Správa potenciálních zákazníků](./manage-leads.md)|

## <a name="next-steps"></a>Další kroky


- [Partner Sales Connect to Partnerské centrum sešit](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) – sešit pro sladění prodejních procesů a rolí partnerů s novými prodejními procesy prostřednictvím Partnerské centrum vs. Partner Sales Connect.
- [Partnerské centrum provozního průvodce](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) spoluprodálováním – pokyny k identifikaci provozního modelu prostřednictvím Partnerské centrum pro správu potenciálních zákazníků nebo příležitostí ke spoluprodání a registraci dohod.
- [Balíček pro správu referenčních](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) doporučení – vizualizované podrobné pokyny ke správě potenciálních zákazníků a příležitostí ke spoluprodání prostřednictvím Partnerské centrum.
- [Publikování](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) a správa na komerčním marketplace – vizualizované podrobné pokyny k vytváření, správě a publikování nabídek prostřednictvím Partnerské centrum na komerčním marketplace.