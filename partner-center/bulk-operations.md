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
ms.openlocfilehash: 8b69b430344c64f3d74e0b5058d561358bdd2b45
ms.sourcegitcommit: d7fbaff51c7ac29fbf700d7f7fdef798fd97c6fa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "102619388"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Hromadné operace pro společný prodej příležitostí pomocí souborů hodnot oddělených čárkami (CSV)

**Příslušné role**

- Správce odkazů
- Uživatel s odkazy

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
- Nemusíte čekat na dokončení akce stahování. I v případě, že přejdete na jiné stránky v partnerském centru, bude soubor stažen ihned po dokončení funkce exportu.
- Stažený soubor můžete znovu použít pro úpravu podrobností o koupi a nahrání pro aktualizaci záznamů.

## <a name="import-co-sell-opportunities"></a>Import příležitostí společného prodeje

- Pomocí funkce Import můžete vytvořit nebo aktualizovat **maximálně 1000 záznamů** .
- Šablonu můžete od začátku vytvořit tak, že stáhnete šablonu ze stránky Import na partnerském centru.
- Můžete také použít funkci exportu ke stažení existujících záznamů a jejich aktualizaci.
- Pokud má soubor více než 1000 záznamů, nelze jej zpracovat.
- Po zpracování souboru se zobrazí souhrn s počtem odkazů, které byly vytvořeny, aktualizovány a zpracovány, na kartě poslední soubor procesu.
- Můžete si stáhnout podrobnosti o zpracovaných záznamech, opravit případné chyby a nahrát stejný soubor pro vytvoření nebo aktualizaci záznamů, které selhaly v předchozím spuštění. **Před nahráním opravených záznamů, které selhaly v předchozím běhu, odeberte ze souboru všechny úspěšné záznamy.**
- Pro přidání dalších řešení přidejte sloupce navíc vedle řešení 1 a použijte název sloupce jako řešení X, kde X představuje číslo řešení v rámci obchodu. Například řešení 2, řešení 3.
- Do obchodu můžete přidat až 50 řešení.
- Pro přidání dalších členů týmu přidejte další sloupce vedle člena týmu 1 a použijte název sloupce jako člen týmu X, kde X představuje číslo člena týmu v obchodu. Příklad: člen týmu 2, člen týmu 3.
- Do koupě můžete přidat až 50 členů týmu.

> [!NOTE]
> Nemusíte čekat na dokončení zpracování. Podrobnosti posledního zpracovaného souboru budou po dokončení zpracování k dispozici ke stažení. **Pokud nahráváte soubory pomocí záznamů 1000, může to trvat až 10 minut.**

> [!IMPORTANT]
> Před vytvořením nebo aktualizací obchodů využívajících soubory CSV v partnerském centru si pečlivě přečtěte všechny pokyny a zkontrolujte formát každého sloupce z tabulky níže.

|**Název sloupce**|**Je povinné?**|**Popis**|**Ukázkové hodnoty**|
|-----|:-----|:---------|:---|
Chyby|No|V tomto sloupci budou zahrnuty chyby související s operacemi Create/Update w. r. t a odkazujícími na odkazy. Pokud dojde k více chybám, budou všechny uvedeny v seznamu oddělené středníkem.|Chybí povinné řešení pole 1.|
ID zapojení|No|ID zapojení je vygenerováno systémem odkazů na partnerském centru společnosti Microsoft. Nepožaduje se pro vytvoření nového odkazu. Pokud aktualizujete záznam, můžete použít existující ID Engagement.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
ID referenčního seznamu|No|ID odkazu je vygenerováno systémem odkazů partnerského centra společnosti Microsoft. Nepožaduje se pro vytvoření nového odkazu. Pokud aktualizujete existující záznam, zadejte ho s ID odkazu.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Název obchodu|Yes|Popisný název obchodu pro referenci.|Koupě spojené s pružinou
Název zákazníka|Yes|Název společnosti zákazníka. Použijte právní název organizace pro rychlé porovnání na straně Microsoftu.|Contoso Corporation
Řádek adresy zákazníka 1|Yes|Adresní řádek 1 zákaznické společnosti. |Jedna z možností contoso
Řádek adresy zákazníka 2|No|Adresní řádek 2 zákaznické společnosti.|No 148 – ulice
Město zákazníka|Yes|Město, kde se nachází organizace zákazníka|Redmond
Stav zákazníka|No|Stát, kde se nachází organizace zákazníka.|Washington
Poštovní směrovací číslo zákazníka|No|Poštovní směrovací číslo oblasti, kde se nachází organizace zákazníka.|98052
Země zákazníka|Yes|Země nebo oblast, kde se nachází organizace zákazníka. Použijte kódy zemí obou písmen, jak je uvedeno [zde]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes).|USA
ID zákazníka D-U-N-S|No|Zkuste načíst ID DUNS organizace zákazníka. To vám pomůže při rychlejším spárování organizace zákazníka na straně Microsoftu, což pomáhá rychleji přiřazovat prodejce. Z tohoto [webu](https://www.dnb.com/duns-number/lookup.html)můžete získat bezplatné ID Duns.|81466849
Křestní jméno kontaktní osoby zákazníka|Závislosti|Křestní jméno je povinné pouze v případě, že potřebujete technickou podporu společnosti Microsoft. Křestní jméno primárního kontaktu od organizace zákazníka, který na této práci pracuje.|John
Příjmení kontaktu zákazníka|Závislosti|Příjmení je povinné jenom v případě, že potřebujete technickou podporu Microsoftu. Příjmení primárního kontaktu od organizace zákazníka, který na této práci pracuje.|Zákazník
Kontaktní telefonní číslo zákazníka|Závislosti|Telefonní číslo je povinné pouze v případě, že potřebujete technickou podporu společnosti Microsoft. Telefonní číslo primárního kontaktu od organizace zákazníka, který na této práci pracuje.|9999999999
Kontaktní e-mailová adresa zákazníka|Závislosti|E-mailová adresa je povinná jenom v případě, že potřebujete podporu Microsoftu. E-mailová adresa primárního kontaktu od organizace zákazníka, která na této práci pracuje.|john.customer@contoso.com
Stav odkazu na partnera|Yes|Označuje stav obchodu z pohledu vaší společnosti. Vyžaduje se, pokud se pokusíte vytvořit nebo upravit odkaz. **Nové** koupě použijte, pokud se pokoušíte vytvořit novou práci. Přijaté hodnoty jsou popsány [zde](/partner/develop/referral-resources#referralstatus).|Aktivní
Podřízený stav odkazu na partnera|Yes|Určuje přesný stav obchodu. Pokud se pokoušíte vytvořit novou práci, použijte **přijato** . Také se vyžaduje, pokud upravujete stávající odkaz. Přijaté hodnoty jsou popsány [zde](/partner/develop/referral-resources#referralsubstatus).|Přijato
Stav odkazů Microsoftu|Závislosti|Označuje stav žádosti o účast v rámci prodeje, který jste odeslali společnosti Microsoft s žádostí o podporu. Toto je pole jen pro čtení. Všechny změny provedené v tomto poli při importu dat budou ignorovány.| Čekající
Důvod zamítnutí/ztráty|Závislosti| Tyto informace je nutné poskytnout pouze v případě, že měníte stav dílčího pole na hodnotu odmítnuto nebo ztraceno. Tento sloupec můžete v opačném případě ignorovat. <br/> **Zadejte číslo na základě níže uvedených možností.** <br/><br/> **1**– projektový rozpočet není adekvátní.  <br/> **2**-zákazník neodpověděl.  <br/> **3**. Zákazník zvolil jiného dodavatele.  <br/> **4** . požadavek zákazníka nebyl splněn.  <br/> **5** – nejedná se o zákazníka. <br/> **6**. Časová osa byla příliš krátká. <br/> **7** . zpráva jako zneužití, spam nebo phishing <br/> **8** – ostatní |6|
Sales Stage|No|Toto pole indikuje detailní prodejní fázi odkazu. Přečtěte si další informace [o fázích](./manage-co-sell-opportunities.md) prodeje.|40
Odhadovaná hodnota koupě|Yes|"Hodnota obchodu na základě počátečních konverzací se zákazníkem. To může být změněno, dokud obchod nedosáhne některého z terminálových stavů.| výhra nebo ztracena. "|12563
Měna|Yes|Měna, ve které se zadá hodnota koupě Kódy měn můžete najít [tady](https://en.wikipedia.org/wiki/ISO_4217).|USD
Odhadované datum ukončení|Yes|Odhadované datum uzavření obchodu na základě počátečních konverzací se zákazníkem ve formátu MM/DD/RRRR. <br/> **Datum by mělo být v časovém pásmu UTC. Všechna data zobrazená v uživatelském rozhraní partnerského centra jsou založená na lokalizovaných časových pásmech. Pokud se díváte na odkaz, pro který jste zadali datum v časovém pásmu UTC, může v uživatelském rozhraní partnerského centra existovat rozdíl za jeden den.**|1/30/2020
ID CRM|No|Identifikátor tohoto konkrétního odkazu v systému CRM, pokud existuje. Toto je textové pole pro zadávání textu v bezplatné formě.|34234324-sdfsdf-345345-SFD
ID marketingové kampaně|No|Toto pole indikuje marketingovou kampaň, která vedla k tomuto konkrétnímu odkazu. Obvykle se používá pro výpočet návratnosti investic.|BingSummer2020
Poznámky|No|Podrobné poznámky, které označují aktualizace související s odkazem|Toto je ukázková Poznámka.
Potřebujete povinnou podporu Microsoftu?|Yes|To je jasné, jestli chcete, aby vám Microsoft pomohly při provádění této žádosti o společný prodej.|Yes
Jakou konkrétní technickou podporu Microsoft?|Závislosti|Jedním ze šesti různých způsobů, jak vám může Microsoft pomáhat. To platí jenom v případě, že pro otázku není vyžadována Nápověda společnosti Microsoft? " <br/> **Zadejte číslo na základě níže uvedených možností.** <br/><br/> **1**– Změna hodnoty specifické pro úlohu  <br/> **2**. Technická architektura pro zákazníky  <br/> **3**. Ověření konceptu/demo  <br/> **4**– kurzy a licencování  <br/> **5**. úspěch zákazníka po prodeji  <br/> **6**– obecné nebo jiné|1|
Sdílení s prodejním týmem Microsoftu|Yes|To znamená, že chcete sdílet podrobnosti o obchodu s prodejním týmem Microsoftu nebo ne. To platí jenom v případě, že pro otázku není vyžadována Nápověda společnosti Microsoft? "|Yes
Poznámky Microsoftu|No|Jakékoli konkrétní poznámky Microsoftu, pokud potřebujete pomáhat od Microsoftu|Potřebujete nápovědu k ověření koncepce pro zákazníka společnosti Contoso
Souhlas s sdílením kontaktu s zákazníkem a partnerem|Yes|Souhlas se sdílením kontaktních údajů zákazníků a pracovníků vaší společnosti s kontaktními údaji, kteří pracují na obchodování. **Pokud pro tento sloupec vyberete možnost Ne, obchody se nevytvoří ani neaktualizují.** |Yes
Řešení 1|Yes|ID řešení (povinné), měna (volitelné), ve které se zadá hodnota koupě [Zde](https://en.wikipedia.org/wiki/ISO_4217)najdete kódy měn, cenu SKU (volitelné) a množství skladové položky (volitelné).  |SOL-1234-PQRS, USD, 10, 100
Člen týmu 1|Yes|Křestní jméno, příjmení, mobilní číslo a ID e-mailu příslušného člena týmu.| Bob, partner, 999999, Bob.partner@Contoso.com

## <a name="next-steps"></a>Další kroky

Tyto konektory v partnerském centru můžete použít pro spoluprodejní práci s Microsoftem v rámci svých systémů CRM.

- [Konektor pro společný prodej pro Dynamics 365 CRM – přehled](connector-dynamics.md)
- [Konektor pro společný prodej pro Salesforce CRM – přehled](connector-salesforce.md)
