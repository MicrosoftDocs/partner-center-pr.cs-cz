---
title: Migrace z partnerského prodejního připojení (PSC)
description: Přečtěte si, jak můžou partneři Microsoftu migrovat z partnerského prodejního připojení (PSC) do partnerského centra a vytvářet nebo spravovat obchody odesílané prodejci Microsoftu.
ms.topic: article
author: vikramb
ms.author: vikramb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/06/2020
ms.openlocfilehash: 34a18e4a4bf4d5c29265fdf76fae05b4ba16a3bc
ms.sourcegitcommit: 445c7b70943f71cc4b2cb48a327b9dcc1814974d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/17/2020
ms.locfileid: "94670163"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Průvodce spoluprodejem v partnerském centru (PC) pro partnery, kteří se migrují z partnerského prodejního připojení (PSC)

**Platí pro**

- Partnerské centrum

**Příslušné role**

- Správce účtu
- Správce odkazů
- Prodejce partnera Sales Connect (PSC)
- Správce PSC (partner Sales Connect)
- Manažer koupě partnera Sales Connect (PSC)

Jak víte, vaše společnost ztratí přístup k 31. března 2021. Najdete ale všechno, co chcete udělat k vytváření spolupracujících obchodů, spravovat své obchody a působit na obchody odeslané prodejci Microsoftu v partnerském centru. V takovém případě budou k dispozici rozdíly a následující doprovodné materiály vám pomůžou přejít k plynulejšímu a přímému přesunu partnerského centra.

>[!Important]
> Pokud jste tady, protože jste si v části PSC o migraci viděli banner, jste na správném místě. Tato příručka se nedá použít pro hodnocení řešení (SA) a pro partnery OEM IOT, kteří spravují své obchody v PBV.

## <a name="before-you-move-things-you-need-to-know"></a>Než přesunete, co potřebujete znát

### <a name="if-you-are-psc-admin"></a>Pokud jste správce PSC

- K přihlášení k [partnerskému centru](https://partner.microsoft.com/)potřebujete pracovní e-mail.
- Nastavte si účet pomocí [správce účtu](permissions-overview.md)partnerského centra.
- Přečtěte si tento dokument a Naučte se, jak v partnerském centru využít společný prodej.
- Nastavte uživatelské účty v partnerském centru pro všechny vaše uživatele PSC (role správce, správce řízení a prodejce) a přiřaďte jim [role Správce odkazů](permissions-overview.md).

>[!Important]
> Ujistěte se, že ID MPN zobrazené v proužku PSC je dostupné v seznamu umístění MPN v partnerském centru. Pokud chcete najít seznam všech MPNs přidružených k účtu partnerského centra, můžete v partnerském centru ověřit kliknutím na nastavení účtu a[umístění](manage-locations.md).

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Obrázek znázorňující hlavičku PSC, kde mohou partneři najít ID MPN.":::

### <a name="if-you-are-psc-deal-manager-or-seller"></a>Pokud jste správce řízení pro správu PSC nebo prodejce

- K přihlášení do [partnerského centra](https://partner.microsoft.com/)potřebujete pracovní e-mail.
- Pokud používáte nepracovní účet v PSC nebo máte pracovní e-mail pro jinou společnost než Partnerská společnost, požádejte správce PSC, aby vám pomohli nastavit účet.
- Pokud je váš účet partnerského centra nastavený na úplný, obraťte se na správce PSC bez ohledu na účet, který používáte k přihlášení k účtu PSC.
- Ověřte, zda máte přístup do partnerského centra a části s odkazy.
- Přečtěte si tento dokument, abyste pochopili pracovní postupy a změny v partnerském centru.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Jako správce v PSC se jedná o vaše další kroky.

Pokud nevidíte kartu odkazy:

- [Globální správce](permissions-overview.md) vaší společnosti vám může udělit přístup k kartě odkazy. Pokud chcete najít globálního správce, v pravém horním rohu partnerského centra se podívejte na nastavení partnerů z ikony ozubeného kola. Na druhé úrovni levého navigačního panelu vyberte stránku správy uživatelů. Klikněte na rozevírací nabídku, která v pravém horním rohu stránky zobrazuje "Všichni uživatelé" a přejděte na globální správci. Na stránce se pak zobrazí všichni globální správci s příslušnými ID e-mailu. Řekněte jim, aby k vašemu pracovnímu účtu získali přístup "Správce odkazů".

  >[!Important]
  > Pokud vaše role spravuje jenom uživatele v účtu PSC, můžete získat roli [správce účtu](permissions-overview.md#manage-mpn-membership-and-your-company) v partnerském centru. Pokud vaše role zahrnuje i správu příležitostí pro společný prodej, měli byste získat roli [Správce odkazů](permissions-overview.md#manage-referrals) . Také je navržený vedoucí změna v rámci správců PBV, aby spolupracovali se správcem účtu v partnerském centru, nikoli všemi správci účtu PSC v počítači individuálně.

  :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="Obrázek znázorňující správce účtu na stránce Správa uživatelů nastavení partnera.":::

- Přejděte na kartu odkazy v levém navigačním podokně a ověřte, jestli máte přístup ke stránkám.

  >[!Note]
  > Možná se budete muset odhlásit z partnerského centra a znovu se přihlásit a aktualizovat přihlašovací údaje pro přístup ke stránkám s odkazy.

## <a name="user-migration"></a>Migrace uživatelů

Po nastavení účtu v partnerském centru můžete pomocí Průvodce migrací uživatelů na stránce příležitosti společného prodeje automaticky přiřadit role partnerského centra zaměstnancům vaší společnosti.

>[!Note]
> Migraci uživatelů můžou provádět jenom [Správci účtu](permissions-overview.md#manage-mpn-membership-and-your-company) vaší společnosti. Pokud nemáte roli správce účtu, najděte správce účtu, který vám může pomáhat nastavit uživatelské účty pomocí Průvodce migrací uživatele. Funkce migrace uživatelů bude k dispozici od 18. listopadu 2020.

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="Obrázek znázorňující Průvodce migrací uživatele":::

Správci účtů získají odkaz Průvodce migrací uživatele PSC na stránce příležitosti společného prodeje vedle Průvodce referenčními postupy. Můžete zahájit migraci uživatelů kliknutím na odkaz. Tuto akci je možné provést několikrát, dokud se všichni uživatelé, kteří chtějí migrovat do společnosti, přiřadí správné role v partnerském centru.

Tabulka migrace uživatelů má následující podrobnosti.

- Uživatelský účet – ID e-mailu zaměstnance
- Partnerský účet PSC – účet, ke kterému je zaměstnanec přidružen v účtu PSC
- PBV role uživatele – jedna ze tří rolí přiřazených do PSC.
- Umístění programu MPN počítače – umístění, pro které se uživateli přidají příslušné role počítačů. Partnerský účet PSČ MPN slouží k vyhledání ekvivalentního umístění programu MPN v partnerském centru za účelem přiřazení oprávnění. Celá organizace označuje ID MPN vOrg.
- POČÍTAČová role uživatele – zaměstnanci jsou přiřazeni role na základě jejich rolí uživatele PBV. Správci v řadiči PSC budou v počítači přiřazeni role správců odkazů. Prodávající bude mít přiřazenou roli uživatele odkazy v počítači. Přečtěte si další informace o rolích počítačů a o tom, co můžou uživatelé s těmito rolemi dělat v partnerském [centru.](permissions-overview.md#manage-referrals)
- POČÍTAČ AAD – tenant, ke kterému se uživatelé přiřazují v partnerském centru
- Stav: stav migrace je tři možné stavy.
    - Nemigrováno – uživatel nemá přiřazenou žádnou roli odkazů na počítače.
    - Migrace – uživatel byl úspěšně migrován s přiřazenou relevantní rolí, jak je znázorněno v tabulce.
    - Chyba: nepovedlo se dokončit migraci kvůli nějaké chybě.

Migrace může selhat a v některých případech dojde k chybám, pro které jsou řešení uvedená níže.

1. Uživatelé PSC můžou používat nepracovní účet.

2. Uživatelé PSC můžou používat účet z domény, která se liší od účtu, který používáte v partnerském centru.

   - Pro řešení chyb souvisejících s scénáři 1 a 2 se všichni tito uživatelé musí přihlašovat do partnerského centra pomocí svého pracovního účtu připojeného k vašemu tenantovi služby Azure AD. Váš [globální správce](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) vám může s tímto. Pokud chcete najít globálního správce, v pravém horním rohu partnerského centra se podívejte na nastavení partnerů z ikony ozubeného kola. Klikněte na stránku správy uživatelů na druhé úrovni levého navigačního panelu. Klikněte na rozevírací nabídku, která v pravém horním rohu stránky zobrazuje "Všichni uživatelé" a přejděte na globální správci. Globální správce může buď vytvořit nový uživatelský účet v tenantovi Azure AD, nebo přiřadit přístup uživatelů typu Host k ostatním uživatelům účtu domény. Jakmile jsou účty nastavené pro všechny správce a uživatele pro řízení účtu PSC, musí se přihlásit k partnerskému centru, přejít na kartu odkaz v levém navigačním panelu a zkontrolovat, jestli uvidí stránku s odkazy.

3. Uživatel už má přiřazenou roli reference v partnerském centru.
    - Existující roli uživatele můžete ověřit na stránce Správa uživatelů v nastavení účtu a podle potřeby upravit.

Po dokončení migrace uživatelů pomocí následujících pokynů určete strategii migrace: 

Pokud má vaše společnost PDM – když je nastavený účet partnerského centra a vaši uživatelé přesunuli a mají role a oprávnění, můžete své spolupracovní aktivity přesunout do partnerského centra. Informujte PDM, aby místo čekání na dokončení migrace nečekala na dokončení migrace. Tím umožníte, aby všechny vaše nové obchody pokračovaly do partnerského centra.

>[!Note]
>Po provedení tohoto přepínače budete moct pracovat jenom s existujícími aktivními obchody v PBV. Nemůžete ani vytvořit nové obchody ani dostávat žádné obchody od prodejců Microsoftu v PBV.

Pokud vaše společnost nemá PDM, ujistěte se, že jsou všechny uživatelské účty nastavené a ověřené všemi uživateli. Budete upozorněni e-mailem a bannerem v části PSC ohledně přesného data, kdy můžete začít prodávat v partnerském centru. Mějte na paměti, že stále budete muset spravovat existující aktivní obchody v PSC.

>[!Important]
>Aktivní obchody nebudou migrovány na počítač. Až do 31. prosince 2020 uzavřete a zaregistrujete obchody.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Další kroky pro správce PSC, správci koupích a PBV

Přečtěte si, jak v partnerském centru využít společný prodej.
Toto je důležitý krok, který vám pomůže připravit se na společný prodej v partnerském centru. Seznamte se s pracovními postupy a změnami v partnerském centru, abyste se mohli efektivně prodávat od prvního dne. Začněte tím, že dokument přečtete úplně. V [galerii možností společného prodeje](https://aka.ms/cosellexperience)jsou k dispozici také dobrá sada prostředků.

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

## <a name="psc-and-partner-center-field-mapping"></a>Mapování polí PSC a partner Center

V této části jsou uvedeny přesné mapování atributů mezi PSC a Partnerským centrem. Každá obrazovka v PBV se porovnává s relevantním zobrazením v části partnerských příležitostí v partnerském centru. 

>[!Note]
>Při hledání ekvivalentního atributu v partnerském centru sledujte čísla žlutých bublin na snímcích obrazovky PBV. Červené bubliny označují, že archivovanou není k dispozici v partnerském centru.

**Domovská stránka PBV a výchozí zobrazení příležitostí společného prodeje v partnerském centru**

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="Obrázek znázorňující mapování polí mezi domovskou stránkou partnera Sales Connect a výchozím zobrazením příležitostí v partnerském centru pro společné prodeje.":::

**Zobrazení mřížky PSC a partnerský pohled centra**

- V partnerském centru neexistuje žádné zobrazení seznamu, jako je třeba PBV.  Všechny obchody jsou uvedené na základě nejnovějšího data přijetí nebo vytvoření s informacemi o zákaznících a typu obchodu. Ve výchozím nastavení je vybrán první obchod v zobrazení. Většina hodnot zobrazených ve formátu tabulky PSC je k dispozici v podrobném zobrazení obchodu v počítači.
- Role koupě není požadované pole v počítači. Není zobrazen ani zachycen v žádném z pracovních postupů. Je odvozená automaticky na straně prodejce Microsoftu na základě řešení přidaných do obchodu.
- Datum poslední změny se nezobrazí na stránce podrobností odkazu v počítači PC. Partneři mohou pomocí funkce řazení seřadit obchody na základě data poslední aktualizace.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Obrázek znázorňující mapování polí mezi zobrazením mřížky partnera Sales Connect (PSC) a zobrazením obchodu v partnerském centru.":::

**Zobrazení podrobností o koupi v PSC a partnerském centru**

- Partneři můžou upravovat práci kliknutím na tlačítko Upravit v zobrazení Podrobnosti o partnerském obchodu pro obchod (6). Jakmile kliknete na tlačítko Upravit, všechna pole se upraví, a to tak, že se uloží nebo zruší úpravy provedené v obchodu.
- Neexistuje možnost uzavřít obchod jako duplicitní v partnerském centru.
- Výsledek zákazníka není v partnerském centru k dispozici. Všechny podrobnosti související s interakcí zákazníků lze aktualizovat v části poznámky v počítači PC.
- Odhadované datum ukončení řešení je k dispozici pouze v partnerském centru pro služby IOT v systému OEM. Nezobrazuje se pro žádné jiné typy obchodování.
- V počítači není vyžadován licenční program. Je automaticky odvozen na základě řešení vybraných v rámci obchodu.

>[!Note]
>Příspěvek, který byl označen jako výhra nebo ztraceno, nelze upravovat. Při přesunu obchodu do jednoho z těchto stavů terminálu Vyzkoušejte opatrnost.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Obrázek znázorňující mapování polí mezi zobrazením podrobností o prodeji partnera Sales Connect (PSC) a zobrazení podrobností pro partnerské Centrum":::

**Zobrazení PSC ' Přidat produkty ' a partnerské Centrum ' Přidat řešení '**

:::image type="content" source="images/pscmigration/products.png" alt-text="Obrázek znázorňující mapování polí mezi zobrazením pro přidání produktů z partnerského prodeje (PSC) a v partnerském centru pro přidání řešení.":::

**Správa uživatelů v PSC a partnerském centru**

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Obrázek znázorňující mapování polí pro domovskou stránku správy uživatelů (PSC) pro partnery a správu uživatelů v partnerském centru v zobrazení nastavení účtu.":::

**Přiřazení role uživatele v PSC a partnerském centru**

- Ekvivalentní role pro správce PSC je role správce účtu v partnerském centru.
- V partnerském centru existuje jenom jedna role pro spoluprodejní správu koupek, což je role Správce odkazů.

:::image type="content" source="images/pscmigration/roles.png" alt-text="Obrázek znázorňující mapování polí mezi zobrazením přiřazení role partnerský prodej Connect (PSC) a zobrazení přiřazení role partnerského centra.":::

**Oznámení v PSC a partnerském centru**

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Obrázek znázorňující mapování mezi oznámeními partnera Sales Connect (PSC) a zobrazením oznámení partnerského centra":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Přesun z PSC do partnerského centra – Nejčastější dotazy

**Dotazu. Co mám dělat, když nemám přístup k partnerskému centru?**

Můžete se obrátit na správce, kteří jsou uvedeni na stránce "bez přístupu", a získat tak přiřazené role. V části referenčních seznamů budete potřebovat roli[Správce odkazů](permissions-overview.md#manage-referrals)pro oprávnění ke čtení a zápisu. Pokud spravujete jenom obchodní profily, budete potřebovat roli správce obchodních profilů v partnerském centru.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Obrázek znázorňující, že v partnerském centru není prostředí pro přístup.":::

**F2. Kdo může udělit přístup k části odkazy v partnerském centru?**

[Správce účtu](permissions-overview.md#manage-mpn-membership-and-your-company) vám může udělit přístup k kartě odkazy. Správce účtu zjistíte tak, že v pravém horním rohu partnerského centra přejdete na nastavení partnerů z ikony ozubeného kola. Klikněte na stránku správy uživatelů na druhé úrovni levého navigačního panelu. Klikněte na rozevírací nabídku, která v pravém horním rohu stránky zobrazuje "Všichni uživatelé" a přejděte na "správci účtů". Na stránce se pak zobrazí všichni správci účtu se svými příslušnými identifikátory e-mailu. Řekněte jim, aby k vašemu pracovnímu účtu získali přístup "Správce odkazů".

**Q3. Tlačítko + nové koupě je pro náš účet šedé. Co mám udělat, pokud chcete začít vytvářet obchody?**

K tomu dochází pouze v případě, že v partnerském centru nejsou k dispozici žádná řešení připravená k prodeji do organizace programu MPN. Kontaktujte PDM a Získejte ID MPN vašich řešení, nebo vytvořte lístek podpory s zmínkou o problému "nové možnosti obchodování po migraci PSC".

**Dotaz. Můžu ke konkrétní osobě přiřadit nějaké obchody z naší organizace, jako je například PSC?**

Členům týmu můžete přiřadit konkrétní obchod. Neblokuje zobrazení ani nefunguje na těchto vzdaných správcích odkazů. 

**Q5. Existuje zobrazení všech obchodů přiřazených mně?**

Můžete použít funkci oblíbené, která je kartou na úrovni uživatele. Všechny obchody, které jsou vám přiřazeny jako oblíbené, můžete označit jako oblíbené a získat tak rychlý přístup k těmto seznámení.

**Q6. Je pro tyto obchody k dispozici zobrazení jen pro čtení?**

Ne, v části referenčních seznamů neexistují žádné zobrazení obchodů jen pro čtení. Všichni správci odkazů budou mít úplný přístup pro čtení a zápis pro všechny obchody.

**Q7. Jak můžu zaregistrovat obchod po jeho výhrě?**

Pokud obchod splňuje níže uvedená kritéria, zobrazí se automaticky otevírané okno pro zahájení [registrace](./register-deals.md).

- Je k dispozici vhodné řešení, které by mělo být spojeno s motivací.
- Prodejce Microsoftu se zve k účasti na obchodování nebo vás pozval k obchodování.
- Karta Microsoft je ve stavu přijato nebo získáno v partnerském centru.

**Q8. Po kliknutí na tlačítko + Nová registrace koupě v části registrace Koupek se zobrazí chybová zpráva. Jak můžu zaregistrovat svoje obchody?**

"+ Nová registrace koupek" je používána pouze partnery, kteří jsou zaregistrovaní v programu ISV Connect pro registraci obchodu bez odpovídající možnosti společného prodeje v partnerském centru. Pro registraci obchodů s příležitostí pro spoluprodeji se zobrazí automaticky otevírané okno, když je práce označena jako získaná a pokud splňuje kritéria pro registraci koupek.

**Q9. Je přidání organizace zákazníka povinné?**

Ano, v partnerském centru je přidání [organizace zákazníka](./manage-co-sell-opportunities.md#select-your-customer) povinné. Začněte tím, že vyhledáte umístění, kde se zákazník nachází. Na základě podrobností, které máte; můžete být specifické, včetně přesného názvu budovy, nebo jenom poskytnout podrobnosti o městech. Hledání v organizaci načte všechny platné entity, které odpovídají názvu, který zadáte, abyste nemuseli zadávat žádné podrobnosti o adrese. Všechny podrobnosti se vyplní automaticky na základě vybrané organizace.

**Q10. Jsou kontaktní údaje zákazníka povinné?**

Závisí na [typu obchodu](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) , kterou vytváříte. Pokud sdílíte svůj kanál a nevyžadujete žádnou technickou podporu z prodejní organizace Microsoftu, můžete se rozhodnout nedávat kontaktní údaje od zákazníka. Pokud společně vydáváte, kde aktivně hledáte pomocníka od společnosti Microsoft, budete muset zadat kontaktní údaje zákazníka. Před vytvořením žádosti o společný prodej v partnerském centru byste měli získat výslovný souhlas od zákazníka.

**Q11. Kolik řešení mohu přidat do obchodu?**

Do obchodu můžete přidat až 50 řešení (podobných produktům v PBV). Na rozdíl od PSC můžete kombinovat řešení ze svých vlastních řešení vhodných pro vlastní prodej, SKU Microsoft First stran a dalších oprávněných řešení pro vlastní prodej třetích stran. V partnerském centru neexistuje žádná role koupě, která by se měla vybrat nebo k dispozici. U položek SKU společnosti Microsoft můžete volitelně přidat množství a cenu za každou SKU, která je do obchodu přidána.

**Q12. Kdy se po vytvoření obchodu získá informace o prodejci Microsoftu?**

Prodejci Microsoftu se přiřazují až po splnění přesného požadavku na podporu, který jste uvedli při vytváření obchodu s relevantním prodejcem na straně Microsoftu. I po přiřazení budou mít prodejci Microsoftu možnost přijmout nebo odmítnout pozvánku pro spoluprodej. V případě, že prodávající akceptuje pozvání k spoluprodeji, bude aktualizace aktualizována o kontaktní údaje prodejce Microsoftu. Smlouva SLA, kterou prodejci Microsoftu budou působit na obchod, je 14 dní. Jedná se o stejnou smlouvu SLA, kterou partneři musí v obchodu řešit předtím, než se do stavu vypršení platnosti.

**Q13. Kde najdu ID příležitosti?**

ID příležitosti v PSC je stejné jako ID koupě v počítači. ID koupě můžete najít vedle názvu obchodu při otevření jakékoli koupě.

**Q14. Jak má PDM získat přístup k počítači?**

Partnerskému centru nemůže mít váš PDM přímý pøístup na rozdíl od PSC. Existuje několik možností, jak tuto funkci povolit, které jsou uvedeny níže.

- OCP Insights – Pokud PDM jenom zobrazujeme obchody & průběh související s nimi, můžou pomocí portálu OCP Insights získat zobrazení vaší organizace. Toto je interní nástroj, který je dostupný jenom pro PDM. Upozorňujeme, že pro uživatele vaší společnosti nejsou k dispozici informace OCP Insights.
- Uživatel typu Host v partnerském centru – účet PDM můžete přidat @microsoft.com jako uživatele typu Host v partnerském centru a přiřadit jim roli správce odkazů, aby mohli zobrazit a pracovat s referenčními seznamy.
- Vytváří se [Nový uživatel](./create-user-accounts-and-set-permissions.md#add-a-new-user) ve vašem tenantovi – můžete vytvořit nového uživatele ve vlastním tenantovi a sdílet tyto podrobnosti s PDM, aby mohli zobrazit a pracovat s odkazy podobnými ostatním uživatelům s odkazem ve vašem účtu.

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

Postupujte podle těchto dalších prostředků:

- [Partner Sales Connect to](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) Workbook – sešit – sešit pro zarovnávání prodejních procesů a rolí partnerů pomocí nových prodejních procesů prostřednictvím partnerského centra vs. partner Sales Connect.
- [Provozní příručka pro partnery v partnerském centru](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) – pokyny k identifikaci operačního modelu prostřednictvím partnerského centra za účelem správy zájemců nebo příležitostí společného prodeje a evidence obchodů.
- [Balíček pro správu referenčních](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) informací – vizuální podrobné pokyny pro správu zájemců a příležitostí k prodeji prostřednictvím partnerského centra.
- [Publikování a správa na komerčním webu Marketplace](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) – vizuální podrobné pokyny k vytváření, správě a publikování nabídek prostřednictvím partnerského centra na komerčním tržišti.
