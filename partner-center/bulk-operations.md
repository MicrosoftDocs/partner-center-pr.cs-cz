---
title: Hromadný export a import příležitostí ze společného prodeje prostřednictvím souborů Excelu/CSV v referenčních seznamech
description: Naučte se stahovat, vytvářet nebo aktualizovat příležitosti pro prodej pomocí souborů aplikace Excel (CSV) v partnerském centru.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: af567b9b8b36841b6e6fd7e18a34e1c4b6b81f2e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149158"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Hromadné operace pro společný prodej příležitostí pomocí souborů hodnot oddělených čárkami (CSV)

**Příslušné role**: Správce odkazů | Uživatel s odkazy

Hromadné operace v partnerském centru vám pomůžou s exportem a importem dat příležitostí do prodeje. Přejděte na stránku **příležitosti společného prodeje** a vyhledejte odkazy na **Import** a **Export** v pravém horním rohu nápisu nadpisu stránky. Tuto funkci můžou používat i uživatelé, kteří mají oprávnění **uživatelů** s odkazy i **Správci** .

> [!IMPORTANT]
> Akce vytvořit nebo aktualizovat provedené prostřednictvím hromadného importu nelze vrátit zpět. Při úpravách nebo vytváření velkého počtu záznamů buďte opatrní. Po vytvoření koupě lze změnit pouze podmnožinu polí. **Žádné akce se nepovolují, jakmile jakákoli koupě dosáhne stavu terminálu, jako je odmítnuto/prošlo/výhra/ztraceno.**

## <a name="export-co-sell-opportunities"></a>Export příležitostí společného prodeje

Následující informace popisují funkce exportu:

- Kliknutím na tlačítko **exportovat** můžete exportovat **maximálně 5000 záznamů** .
- Stažené obchody budou založené na úrovních přístupu. Správci odkazů a referenční uživatelé mohou získat různé výsledky na základě jejich oboru a zahrnout je jako členy týmu v rámci obchodů. Přečtěte si další informace o [oprávněních odkazů](permissions-overview.md#manage-referrals).
- Funkce exportu vezme v úvahu aktuální kartu na stránce příležitosti společného prodeje a použité filtry.
- Vygeneruje se soubor CSV se všemi daty založenými na použitých filtrech.
- Stažení záznamů může trvat až jednu minutu.
- Nemusíte čekat na dokončení akce stažení. I když přejdete na jiné stránky Partnerské centrum, soubor se stáhne, jakmile se funkce exportu dokončí.
- Stažený soubor můžete opakovaně použít k úpravě podrobností o dohody a k nahrání a aktualizaci všech záznamů.

## <a name="import-co-sell-opportunities"></a>Příležitosti ke spoluprodání importu

- Pomocí funkce importu můžete vytvořit nebo aktualizovat maximálně **1 000** záznamů.
- Šablonu můžete vytvořit od začátku tak, že šablonu stáhnete ze stránky Import na Partnerské centrum.
- Pomocí funkce Export můžete také stáhnout existující záznamy a aktualizovat je.
- Pokud má soubor více než 1 000 záznamů, nelze ho zpracovat.
- Po zpracování souboru se na kartě posledního procesu zobrazí souhrn s počtem vytvořených, aktualizovaných a nezpracujených referenčních odkazů.
- Můžete si stáhnout podrobnosti o zpracovaných záznamech, opravit případné chyby a nahrát stejný soubor a vytvořit nebo aktualizovat záznamy, které selhaly v předchozím spuštění. **Před odesláním opravených záznamů, které selhaly při předchozím spuštění, odeberte ze souboru všechny úspěšné záznamy.**
- Pokud chcete přidat další řešení, přidejte vedle řešení 1 další sloupce a použijte název sloupce jako Řešení X, kde X představuje číslo řešení v dohody. Například Řešení 2, Řešení 3.
- Do dohody můžete přidat až 50 řešení.
- Pokud chcete přidat další členy týmu, přidejte další sloupce vedle položky Člen týmu 1 a použijte název sloupce jako člena týmu X, kde X představuje počet členů týmu v dohody. Například člen týmu 2, člen týmu 3.
- Do dohody můžete přidat až 50 členů týmu.

> [!NOTE]
> Nemusíte čekat na dokončení zpracování. Podrobnosti o posledním zpracovaném souboru budou po dokončení zpracování k dispozici ke stažení. **Pokud nahráváte soubory s 1 000 záznamy, může to trvat až 10 minut.**

> [!IMPORTANT]
> Před vytvořením nebo aktualizací obchodů využívajících soubory CSV v partnerském centru si pečlivě přečtěte všechny pokyny a zkontrolujte formát každého sloupce z tabulky níže.

|**Název sloupce**|**Je povinné?**|**Popis**|**Ukázkové hodnoty**|
|-----|:-----|:---------|:---|
Chyby|No|V tomto sloupci budou zahrnuty chyby související s operacemi Create/Update w. r. t a odkazujícími na odkazy. Pokud dojde k více chybám, budou všechny uvedeny v seznamu oddělené středníkem.|Chybí povinné řešení pole 1.|
ID zapojení|No|ID zapojení je vygenerováno systémem odkazů na partnerském centru společnosti Microsoft. Nepožaduje se pro vytvoření nového odkazu. Pokud aktualizujete záznam, můžete použít existující ID Engagement.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
ID referenčního seznamu|No|ID odkazu je vygenerováno systémem odkazů partnerského centra společnosti Microsoft. Nepožaduje se pro vytvoření nového odkazu. Pokud aktualizujete existující záznam, zadejte ho s ID odkazu.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Název obchodu|Yes|Popisný název obchodu pro referenci.|Koupě spojené s pružinou
Název zákazníka|Yes|Název společnosti zákazníka. Použijte právní název organizace pro rychlé porovnání na straně Microsoftu.|Contoso Corporation
Řádek 1 adresy zákazníka|Yes|Adresní řádek 1 zákaznické společnosti |One Contoso Way
Řádek 2 adresy zákazníka|No|Adresovat řádek 2 zákaznické společnosti.|NE 148 street
Customer City|Yes|Město, kde se nachází organizace zákazníka.|Redmond
Customer State|No|Stav, ve kterém se nachází organizace zákazníka|Washington
PSČ zákazníka|No|PSČ oblasti, ve které se nachází organizace zákazníka.|98052
Customer Country|Yes|Země/oblast, ve které se nachází organizace zákazníka. Použijte dvousmenné kódy zemí, jak je uvedeno [tady.]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)|USA
ID zákazníka D-U-N-S|No|Zkuste načíst ID SÍTĚ DUNS organizace zákazníka. To vám pomůže rychleji zajistit shodu organizace zákazníků na straně Microsoftu, což pomáhá rychleji při přiřazování prodejců. Z tohoto [webu](https://www.dnb.com/duns-number/lookup.html)můžete získat bezplatné ID Duns.|81466849
Křestní jméno kontaktní osoby zákazníka|Závislosti|Křestní jméno je povinné pouze v případě, že potřebujete technickou podporu společnosti Microsoft. Křestní jméno primárního kontaktu od organizace zákazníka, který na této práci pracuje.|John
Příjmení kontaktu zákazníka|Závislosti|Příjmení je povinné jenom v případě, že potřebujete technickou podporu Microsoftu. Příjmení primárního kontaktu od organizace zákazníka, který na této práci pracuje.|Zákazník
Kontaktní telefonní číslo zákazníka|Závislosti|Telefonní číslo je povinné pouze v případě, že potřebujete technickou podporu společnosti Microsoft. Telefonní číslo primárního kontaktu od organizace zákazníka, který na této práci pracuje.|9999999999
Kontaktní e-mailová adresa zákazníka|Závislosti|E-mailová adresa je povinná jenom v případě, že potřebujete podporu Microsoftu. E-mailová adresa primárního kontaktu od organizace zákazníka, která na této práci pracuje.|john.customer@contoso.com
Stav odkazu na partnera|Yes|Označuje stav obchodu z pohledu vaší společnosti. Vyžaduje se, pokud se pokusíte vytvořit nebo upravit odkaz. **Nové** koupě použijte, pokud se pokoušíte vytvořit novou práci. Přijaté hodnoty jsou popsány [zde](/partner/develop/referral-resources#referralstatus).|Aktivní
Podřízený stav odkazu na partnera|Yes|Určuje přesný stav obchodu. Pokud se pokoušíte vytvořit novou práci, použijte **přijato** . Také se vyžaduje, pokud upravujete stávající odkaz. Přijaté hodnoty jsou popsány [zde](/partner/develop/referral-resources#referralsubstatus).|Přijato
Stav odkazů Microsoftu|Závislosti|Označuje stav žádosti o účast v rámci prodeje, který jste odeslali společnosti Microsoft s žádostí o podporu. Toto je pole jen pro čtení. Všechny změny provedené v tomto poli při importu dat budou ignorovány.| Čekající
Důvod zamítnutí/ztráty|Závislosti| Tyto informace je nutné poskytnout pouze v případě, že měníte stav dílčího pole na hodnotu odmítnuto nebo ztraceno. Tento sloupec můžete v opačném případě ignorovat. <br/> **Zadejte číslo na základě níže uvedených možností.** <br/><br/> **1**– projektový rozpočet není adekvátní.  <br/> **2**– Zákazník neodpoví  <br/> **3.** Zákazník zvolil jiného dodavatele  <br/> **4** . Požadavek zákazníka není splněný  <br/> **5.** Není zákazníkem <br/> **6**– Navrhovaná časová čára byla příliš krátká <br/> **7.** Nahlásit jako zneužití, spam nebo phishing <br/> **8** - Ostatní |6|
Sales Stage|No|Toto pole označuje podrobnou fázi prodeje referenčního seznamu. Další informace o fázích prodeje [najdete tady.](./manage-co-sell-opportunities.md)|40
Odhadovaná hodnota dohody|Yes|Hodnota dohody na základě počátečních konverzací se zákazníkem. To se může změnit, dokud dohoda nedosáhne jednoho z terminálových **stavů,** které vyhrály nebo **neztratily.**|12563
Měna|Yes|Měna, ve které je zadaná hodnota dohody. Kódy měn najdete [tady.](https://en.wikipedia.org/wiki/ISO_4217)|USD
Odhadované datum uzavření|Yes|Odhadované datum uzavření dohody na základě počátečních konverzací se zákazníkem ve formátu MM/DD/RRRR. <br/> **Datum by mělo být v časovém pásmu UTC. Všechna data zobrazená v uživatelském rozhraní Partnerské centrum založená na lokalizovaných časových pásmech. Pokud se díváte na referenční seznam, pro který jste datum v časovém pásmu UTC zadali, může být v uživatelském rozhraní služby Partnerské centrum rozdíl +/- jeden den.**|1/30/2020
CRM ID|No|Identifikátor tohoto konkrétního referenčního seznamu v systému CRM, pokud je k nějakému dojde. Toto je textové pole volného tvaru.|34234324-sdfsdf-345345-sfd
ID marketingové kampaně|No|Toto pole označuje marketingovou kampaň, která vedlo k tomuto konkrétnímu referenčnímu seznamu. Obvykle se používá pro výpočet návratnosti investic.|BingSummer2020
Poznámky|No|Podrobné poznámky týkající se aktualizací souvisejících s referenčním seznamem|Toto je ukázková poznámka.
Je potřeba pomoc Microsoftu?|Yes|To znamená, jestli vám Microsoft má s vytvořením této žádosti o spoluprodát pomoct.|Yes
Jaká konkrétní nápověda od Microsoftu?|Závisí|Jeden ze šesti různých způsobů, jak vám může Microsoft pomoct. To se vztahuje jenom v případě, že u otázky "Vyžaduje se nápověda Microsoftu?", vyberete Ano. " <br/> **Zadejte číslo na základě následujících možností.** <br/><br/> **1**. Úloha – návrh konkrétní hodnoty  <br/> **2.** Technická architektura zákazníka  <br/> **3.** Doklad o konceptu /Ukázka  <br/> **4**. Uvozovky a licencování  <br/> **5**. úspěch zákazníka po prodeji  <br/> **6**– obecné nebo jiné|1|
Sdílení s prodejním týmem Microsoftu|Yes|To znamená, že chcete sdílet podrobnosti o obchodu s prodejním týmem Microsoftu nebo ne. To platí jenom v případě, že pro otázku není vyžadována Nápověda společnosti Microsoft? "|Yes
Poznámky Microsoftu|No|Jakékoli konkrétní poznámky Microsoftu, pokud potřebujete pomáhat od Microsoftu|Potřebujete nápovědu k ověření koncepce pro zákazníka společnosti Contoso
Souhlas s sdílením kontaktu s zákazníkem a partnerem|Yes|Souhlas se sdílením kontaktních údajů zákazníků a pracovníků vaší společnosti s kontaktními údaji, kteří pracují na obchodování. **Pokud pro tento sloupec vyberete možnost Ne, obchody se nevytvoří ani neaktualizují.** |Yes
Řešení 1|Yes|ID řešení (povinné), měna (volitelné), ve které se zadá hodnota koupě [Zde](https://en.wikipedia.org/wiki/ISO_4217)najdete kódy měn, cenu SKU (volitelné) a množství skladové položky (volitelné).  |SOL-1234-PQRS, USD, 10, 100
Člen týmu 1|Yes|Křestní jméno, příjmení, mobilní číslo a ID e-mailu příslušného člena týmu.| Bob, partner, 999999, Bob.partner@Contoso.com

## <a name="next-steps"></a>Další kroky

Tyto konektory v partnerském centru můžete použít pro spoluprodejní práci s Microsoftem v rámci svých systémů CRM.

- [Konektor pro společný prodej pro Dynamics 365 CRM – přehled](connector-dynamics.md)
- [Konektor pro společný prodej pro Salesforce CRM – přehled](connector-salesforce.md)
