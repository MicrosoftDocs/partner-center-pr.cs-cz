---
title: Oznámení z dubna 2021
description: Oznámení z dubna 2021 pro microsoft Partnerské centrum, včetně nových možností, propagačních akcí, nabídek, trhů nebo změn stávajících nabídek.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 13b8ec9ddd82b38a265606809b8c39c07436e548
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150127"
---
# <a name="april-2021-announcements"></a>Oznámení z dubna 2021

Tato stránka obsahuje oznámení pro Microsoft Partnerské centrum pro duben 2021.

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a>Připravenost: Aktualizované rozhraní API pro ověřování adres zákazníků CSP bude živě k červnu. možnost testování je nyní k dispozici

### <a name="categories"></a>Kategorie

- Datum: 30. 4. 2021
- Připravenost

### <a name="summary"></a>Souhrn

Aby partneři a zákazníci mohli na základě důvěryhodnosti podnikat, vyzveme partnery k otestování změn rozhraní API pro ověřování adres pro všechny země po celém světě.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři CSP s přímým vyúčtováním a nepřímí poskytovatelé, kteří vytvářejí nové nebo aktualizují podrobnosti adresy stávajících zákazníků

### <a name="details"></a>Podrobnosti

Microsoft běží na vztahu důvěryhodnosti. Zavázali jsme se poskytovat vyhovující, bezpečnou a zabezpečenou metodu ověřování adres zákazníků pro transakce s předplatným zákazníků v programu CSP. Od 31. března 2021 jsme zavedli změny rozhraní API pro ověřování adres. Zvou partnery k otestování rozhraní API před jeho zahájením na konci června 2021. 

Tyto změny mají vliv pouze na rozhraní API pro ověření adresy. Na rozhraní API pro vytvoření zákazníka a aktualizaci fakturačního profilu to nebude mít vliv. I když se navrhovaná adresa v současné době nemusí používat s rozhraním API pro vytvoření zákazníka, důrazně se doporučuje.

Odpověď vrátí jednu z následujících stavových zpráv:

| Status     | Popis |    Počet vrácených navrhovaných adres |
|-------|---------------|-------------------|
|Ověřená expedice | Adresa je ověřená a je možné ji poslat na adresu . | Jednoduché |
|Ověřují | Adresa je ověřena. | Jednoduché |
|Je vyžadována interakce | Navrhovaná adresa se významně změnila a potřebuje potvrzení uživatele. | Jednoduché |
|Částečně ulice | Daná ulice v adrese je částečně a potřebuje další informace. | Více – maximálně tři |
|Částečně místní | Dané prostory (stavební číslo, číslo sady a další) jsou částečné a vyžadují další informace. | Více – maximálně tři |
|Několik | Adresa obsahuje několik polí, která jsou v této adrese částečně (případně i částečně a částečně v ulici). | Více – maximálně tři |
|Žádná | Adresa je nesprávná. | Žádná |
|Není ověřeno. | Adresu nelze odeslat prostřednictvím procesu ověřování. | Žádná |

PSČ US vrátí další čtyři číslice a pomlčku, například 12345-6789.

### <a name="next-steps"></a>Další kroky

- Podrobnější pokyny najdete v technické dokumentaci a nejčastější dotazy v [kolekci vyhrazených partnerů](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) .
- Připravte se na začlenění změn pomocí rozhraní API partnerského centra a uživatelského prostředí pro web. 
- Sdílejte své ID tenanta izolovaného prostoru s odborníkem na danou problematiku (Ali pískově), abyste mohli začít připravovat aktualizaci. 
- Pokud používáte řešení v rámci ovládacího panelu (CPV), obraťte se na CPV.

### <a name="questions"></a>Máte otázky?

Pokud potřebujete podporu pro vaše operace s Microsoftem, obraťte se na svého partnera, který podporuje Yammer, nebo otevřete [žádost o služby](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>Nové umístění pro dokumentaci Partnerské centrum API Swagger

### <a name="categories"></a>Kategorie

- Datum: 26. 4. 2021
- Možnosti

### <a name="summary"></a>Souhrn

Partnerské centrum swaggeru s rozhraním API byly migrovány z předchozího webu dokumentace [Swaggeru](https://apidocs.microsoft.com/services/partnercenter) na [nový web dokumentace Swaggeru.](/rest/api/partner-center-rest/)

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři s přímým vyúčtováním a nepřímí poskytovatelé, kteří se účastní programu Cloud Solution Provider (CSP), kteří používají rozhraní API Partnerské centrum rozhraní API

### <a name="details"></a>Podrobnosti

Od 26. dubna 2021 se dokumentace Partnerské centrum API Swaggeru, včetně obsahu rest API, nachází na [novém webu](/rest/api/partner-center-rest/). Starý web bude po několika týdnech nedostupný.

### <a name="benefits"></a>Výhody

V Partnerské centrum API Swaggeru najdete funkci **Try It.** Pokud chcete tuto funkci použít, budete potřebovat bearer token, který můžete vygenerovat pomocí kroků uvedených [v části Partnerské centrum Authentication](/partner-center/develop/partner-center-authentication#app--user-authentication).

### <a name="next-steps"></a>Další kroky

Sdílejte tyto informace v rámci vaší organizace, aby příslušný tým mohl zkontrolovat a aktualizovat své procesy.

### <a name="questions"></a>Máte otázky?

Pokud máte dotazy k těmto nabídekm, podívejte se na příslušné komunity Yammeru.

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a>Cloud Solution Provider doby vracení softwaru (CSP) a stažení oznámení o vypršení platnosti odkazu

### <a name="categories"></a>Kategorie

- Datum: 21. 4. 2021
- Možnosti

### <a name="summary"></a>Souhrn

Došlo ke změnám zásad období vracení softwaru CSP a vypršení platnosti odkazu ke stažení.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři, kteří v CSP provádí transakce s nabídkami časově neomezeného softwaru nebo předplatného softwaru

### <a name="details"></a>Podrobnosti

Všimněte si následujících důležitých oznámení týkajících se nákupů časově neomezeného softwaru a softwarového předplatného prostřednictvím Partnerské centrum:

#### <a name="software-return-period-policy"></a>Zásady období vrácení softwaru

Od 1. června 2021 se doba vrácení softwarových nabídek v PROGRAMU CSP uvedená v programu Smlouva s partnerem Microsoftu (MPA) změní z 60 dnů od data objednávky na 30 dnů od data objednávky.

Po odeslání objednávky softwarové nabídky budou mít partneři 30 dnů od data objednávky, aby mohli odeslat jakékoli revize této objednávky:

- Veškerá Trvalá softwarová licence, která se vrátila během 30denní zpáteční lhůty, obdrží plný kredit placené nákupní ceny.

- Veškerý produkt pro předplatné softwaru vrácený během 30denní zpáteční lhůty obdrží poměrný kredit placené nákupní ceny.

Tato zpráva je následná pro naši e-mailovou komunikaci odeslanou od prosince 2020 do dubna 2021 všem partnerům CSP v souvislosti s návratovou dobou a dalšími aktualizacemi aktivace. V těchto oznámeních najdete úplné podrobnosti o změnách, které mají vliv na aktivaci.

#### <a name="software-download-link-expiry"></a>Vypršení platnosti odkazu na stažení softwaru

Od 3. června 2021 budou odkazy na stažení softwaru pro trvalé nákupy softwaru a softwaru prostřednictvím partnerského centra mít datum vypršení platnosti 5 dní od prvotního stažení. Doba platnosti se bude vztahovat na všechny nákupy do 3. června 2021 a taky do 3. června 2021.

### <a name="next-steps"></a>Další kroky

Přečtěte si [Nejčastější dotazy k návratové době CSP a Stáhněte si informace o vypršení platnosti odkazů](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)a informujte všechny příslušné týmy ve vaší organizaci s těmito změnami:

### <a name="questions"></a>Máte otázky?

Otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a>Otevřený licenční program: přechod prodejců do programu Cloud Solution Provider (CSP)

### <a name="categories"></a>Kategorie

- Datum: 2021-04-19
- Rozšiřte svou firmu

### <a name="summary"></a>Souhrn

Tato komunikace podrobně popisuje, jak připravit změny, které se připravují do programu Open Licensing.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

CSP a Open License partneři

### <a name="details"></a>Podrobnosti

V 2020 společnost Microsoft [oznámila](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) , že trvalé licence k softwaru budou široce dostupné partnerům a zákazníkům prostřednictvím programu Cloud Solution Provider (CSP). První milník byl dosažen v lednu 2021, kdy byly k dispozici komerční nabídky s trvalou dostupností softwaru. Další klíčový milník bude probíhat v červenci 2021, když budou nabídky [veřejného sektoru](https://aka.ms/openlicensepublicsector) k dispozici. Také jsme [komunikovali](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) s účinností od 1. ledna 2022, žádného nového nákupu licence k softwaru ani obnovení programu Software Assurance nebo online služby lze provést prostřednictvím Open License programu.

Přechod trvalého softwaru na program CSP v novém komerčním prostředí pomůže partnerům rozšířit příležitosti k nabídce různých řešení a spravovaných služeb. Tím se také urychlí přechod zákazníků do cloudu.  Pro zajištění hladkého přechodu pro naše partnery i zákazníky jsme provedli tyto úpravy a materiály, které tuto digitální transformaci urychlují:

#### <a name="april-2021"></a>Duben 2021

[Nyní k](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)dispozici: Open License převodní materiály mezi CSP pro prodejce

#### <a name="july-2021"></a>Červenec 2021

##### <a name="csp"></a>CSP

- 1. července: Časově neomezené softwarové licence dostupné zákazníkům z veřejného sektoru

- 7. července: Visual Studio pro a získat časově neomezené softwarové licence pro smlouvu Windows dostupné pro všechny segmenty

##### <a name="open-value"></a>Open Value

- 1. července: Další SKU dostupné v programu Open Value pro vzdělávání a neziskové organizace poskytující podobné nabídky jako Open License program

##### <a name="open-license"></a>Open License

- 1. července: Microsoft už nebude spouštět nové nabídky v Open License programu.

#### <a name="january-2022"></a>Leden 2022

- 1. ledna: Prostřednictvím tohoto programu není možné nic nakupovat ani prodlužovat Open License.

### <a name="next-steps"></a>Další kroky

#### <a name="csp-indirect-providers"></a>Nepřímí poskytovatelé CSP

Následující měsíce vám pomůžou se Open License programu CSP tím, že se zúčastní akcí komunity partnerů a využijí materiály pro převod mezi partnery Open License-CSP pro prodejce:

- [Open License-to-CSP](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)pro prodejce – Přizpůsobitelné prezentace s přehledem, e-mailová šablona, průvodce onboardingem nepřímých prodejců CSP a další materiály, které vám pomůžou při přechodu na vaše prodejce ve velkém měřítku.

- [Komunitní akce partnerů CSP](https://globalpbocomm.eventbuilder.com/GlobalCSP) hostované oddělením Microsoft Business Operations  Připojte se k různým relacím a seznamte se se základy CSP (Základy CSP) nebo se učte být aktuální a ptejte se na software v PROGRAMU CSP (Q&A Sessions).

- (Připravujeme) Školení zaměřené na nepřímé prodejce CSP hostované v Microsoft Business Operations

#### <a name="open-license-resellers"></a>Open License prodejci

- Pokud vaše organizace není v tuto chvíli zaregistrovaná v programu CSP, obraťte se na svého distributora, kde najdete informace o tom, jak začít. [Tady](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)se připojte přímo k poskytovateli.

- Pokud je vaše organizace už zaregistrovaná v programu CSP, další informace o trvalém softwaru v CSP najdete [tady](https://partner.microsoft.com/resources/collection/software-in-csp).

### <a name="questions"></a>Máte otázky?

Další otázky k těmto nabídkám najdete v příslušných komunitách Yammeru.

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a>Nyní Live: Průvodce globální propagační připravenosti

### <a name="categories"></a>Kategorie

- Datum: 2021-04-16
- Možnosti

### <a name="summary"></a>Souhrn

Připravenost na spuštění publikovala nový [Průvodce globální propagační připravenosti](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) v galerii prostředků připravenosti na operace. Tato příručka nabízí konsolidované zobrazení všech aktivních [globálních propagačních akcí](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Všechny multilicenční partneři (VL), Dynamics ceníků (DPL) a poskytovatelé Cloud Solution Provider (CSP)

### <a name="details"></a>Podrobnosti

Partneři Microsoftu sdíleli s námi potřebu získat konsolidované zobrazení všech globálních propagačních akcí s podpůrnými podrobnostmi. Chtěli jste mít k dispozici tuto konsolidovanou příručku, která vám pomůže s tím, že všechny dostupné informace budou snadno přístupné v centrálním a praktickém umístění.

Od dubna 2021 Microsoft tuto příručku po měsících aktualizuje a bude k dispozici v galerii prostředků připravená globální akce v galerii prostředků připravenosti na operace.

Odkazy na tento průvodce budou také zahrnuty v následujících kolekcích:

- [Spustit kolekci kalendáře](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), která poskytuje centralizované zobrazení nadcházejících změn a spuštění.

- [Komunitní kolekce](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), které obsahují podpůrné materiály pro naše měsíční hovory, zvýrazňování nadcházejících změn a včasných témat o provozu.

- [Partnerské zpravodaje](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), jako je měsíční aktualizace CSP

V rámci měsíčního připomenutí zveřejníme také oznámení partnerského centra s každým novým problémem Průvodce globální propagační akce.

### <a name="next-steps"></a>Další kroky

Na začátku každého měsíce najdete nejnovější [Průvodce globálními propagačními](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) akcemi v [galerii prostředků připravenosti na operace](https://partner.microsoft.com/resources).

Podělte se o tyto informace s příslušnými kontakty ve vaší organizaci a dejte nám vědět, jak užitečná je příručka prostřednictvím stránky Bylo to užitečné? na konci každé stránky.

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>Aktualizace a připomenutí Cloud Solution Provider (CSP) z dubna

### <a name="categories"></a>Kategorie

- Datum: 16. 4. 2021
- Komunitní | Pozvánky a připomenutí

### <a name="summary"></a>Souhrn

Komunitní zdroje CSP jsou k dispozici na vyžádání a každý měsíc se aktualizují, abyste byli informováni a připraveni na změnu v programu CSP.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři CSP s přímým vyúčtováním a nepřímí poskytovatelé

### <a name="details"></a>Podrobnosti

Tento měsíc prostředky obsahují následující klíčová témata:

- [Aktualizace vývoje programu CSP a Open License změn programu](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [Změny požadavků na onboarding zákazníků CSP v určitých oblastech](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [Nový formát pro novou fakturu ve formátu PDF obchodu v programu CSP](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

V [komunitní kolekci CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)najdete:

- Bulletin [CSP Monthly Update](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)ke stažení, který v snadno čitelném dokumentu agreguje nejnovější oznámení, aktualizace, události a připomenutí CSP.

- Kalendář [oznámení CSP,](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)který poskytuje zobrazení časové osy nadcházejících změn, které mají vliv na program.

- Nový kalendář [uvedení produktu na trh,](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)kde si můžete prohlédnout nadcházející uvedení produktu na trh a nabídky.

- [CSP spouští aktualizační prostředky](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) se snadno použitelným obsahem o klíčových provozních změnách.

- [Aktualizace a připomenutí klíčových](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) témat CSP, která chystá zájem a dotazy

#### <a name="csp-community-call-qas"></a>CSP Community Call Q&As

Community Call Q&As jsou k dispozici, aby vám pomohly s dotazy souvisejícími s nadcházejícími změnami. Zaregistrujte se hned&volání komunity CSP, jak se provádí v dubnu, květen a červnu. Budou se soustředit na nejnovější spuštění, důležité aktualizace a připomenutí.

[Zaregistrujte se sem](https://globalpbocomm.eventbuilder.com/GlobalCSP).

### <a name="next-steps"></a>Další kroky

Projděte si materiály komunity a zaregistrujte se na dotaz&pro komunitu.

Abyste se ujistili, že získáte maximum z&, přečtěte si obsah komunity na vyžádání a odešlete své dotazy až 48 hodin před voláním.

### <a name="questions"></a>Máte otázky?

Toto je nejlepší místo pro otázky související se změnami v programu CSP, který představuje měsíční volání&komunity poskytovatele CSP. Každý měsíc si Projděte materiál a odešlete své otázky předem, abychom mohli strávit relaci v tématech, která jsou pro vás nejdůležitější.

Pokud chcete získat další informace, obraťte se na [podporu](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>Konečné připomenutí: vyřazení získání kvalifikace z května 6, 2021

### <a name="categories"></a>Kategorie

- Datum: 2021-05-04

- Možnosti

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři, kteří prodávají akademické a neziskové a státní komunitní Cloud (RSZ) prostřednictvím programu Cloud Solution Provider pomocí rozhraní API partnerského centra

### <a name="details"></a>Podrobnosti

Toto oznámení je následná vylepšení partnerského centra [vydané v prosinci](./2020-december.md#1). V rámci této verze se nasadila nová rozhraní API GET a POST a v důsledku toho se **stávající kvalifikace Get vyřadí do 6. května 2021**. V tuto chvíli se budete muset převést na použití nového rozhraní API pro POST Center. Nová rozhraní API pro odesílání vám umožní koupit nabídky vzdělávání, zatímco nové rozhraní API pro získání vám umožní koupit předem kvalifikované nabídky a nabídky RSZ.

### <a name="next-steps"></a>Další kroky

- **Aktualizujte nové rozhraní API** pro úspěšný a včasný přechod.

- **Projděte si nové změny a příručka k rozhraní API partnerského centra** v prostředcích připravenosti operací: [vylepšení procesu ověřování zákazníků z partnerského centra](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).

- Tyto informace můžete sdílet s příslušnými týmy ve vaší organizaci a prodejci, kteří jim pomůžou tyto změny připravit.

### <a name="questions"></a>Máte otázky?

Pokud máte dotazy související s tímto oznámením, obraťte se na [podporu partnerského centra](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).

### <a name="change-log"></a>Protokol změn

- 4. května 2021: Závěrečné připomenutí nadcházejícího vyněcování kvalifikace GET

- 9. dubna 2021: Připomenutí nadcházejícího vyněcování kvalifikace GET 

- Únor: Aktualizace časových os pro vyněcování kvalifikace GET & PUT

- Leden: Připomenutí nadcházejícího vynětu kvalifikace GET & PUT

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a>Nový formát pro novou fakturu ve formátu PDF s komerčním obchodováním v CSP

### <a name="categories"></a>Kategorie

- Datum: 5. 4. 2021
- Možnosti

### <a name="summary"></a>Souhrn

Microsoft zavádí nový formát nové faktury za obchod ve formátu PDF v programu Cloud Solution Provider (CSP), aby se místo popisu skladové položky místo podrobností o produktu zobrazují podrobnosti o fakturaci.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři, kteří provádí transakce prostřednictvím programu CSP

### <a name="details"></a>Podrobnosti

Od května 2021 microsoft zavádí nový formát nové faktury za obchod ve formátu PDF v programu CSP, aby se místo popisu SKU místo podrobností o produktu zobrazují podrobnosti o fakturaci. S touto novou aktualizací budeme agregovat řádkové položky podle typu produktu a současně budeme zobrazovat každý produkt na samostatném řádku.

Partneři si všimnou, že se tato změna projeví na své květnové faktuře za fakturační období od 1. dubna 2021 do 30. dubna 2021. Ovlivněné nabídky jsou Microsoft Azure instance, předplatná Azure (plán Azure) a Marketplace.

Všechny žádosti o opětovné vystavení kreditu provedené po aktualizaci formátu faktury se vygenerují v novém formátu.

#### <a name="partner-benefits"></a>Partnerské výhody

Tato aktualizace nabídne partnerům následující vylepšení možností fakturace:

- Snížení velikosti faktury při zachování důležitých dat

- Sladění formátu s oborové standardy pro kompaktní a uživatelsky přívětivé faktury 

Následující prvky nebudou ovlivněny:

- Stránka souhrnu fakturace na faktuře VE FORMÁTU PDF

- Existující fakturační rozhraní API

- Soubory pro odsouhlasení (soubory rekognoskaci se dají použít k načítání podrobných dat) 

- Používání a fakturování poplatků na základě licencí

### <a name="next-steps"></a>Další kroky

Projděte si informace o tomto tématu v [galerii prostředků připravenosti operací](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) na webu Microsoft Partner. Další informace o fakturačních a daňových tématech, včetně fakturačních prostředků, faktur, fakturace CSP a daní, najdete v [části fakturace](../billing.md) v partnerském centru.

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a>Změny požadavků na registraci zákazníků poskytovatele Cloud Solution Provider (CSP)

### <a name="categories"></a>Kategorie

- Datum: 2021-04-02
- Nabídky/trhy

### <a name="summary"></a>Souhrn

V rámci našeho závazku pomáhat partnerům a zákazníkům, kteří provozují své podnikání na základě důvěry, budeme požadovat další informace o zákaznících, účinnost 25. března 2021.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři poskytovatele CSP a nepřímá poskytovatelé, kteří mají nové nebo existující zákazníky v zemích uvedených v další části

### <a name="details"></a>Podrobnosti

Microsoft běží na důvěryhodnosti. Zavázali jsme se poskytovat vyhovující, bezpečné a zabezpečené metody ověřování zákazníků pro transakce předplatných zákazníka v programu CSP. 25. března 2021 budeme zavádět vylepšení rozhraní API partnerského centra a uživatelského rozhraní, které bude mít vliv na partnery, kteří splňují obě následující kritéria:

- Partner má přímý fakturační vztah s Microsoftem (to znamená, že partner je buď přímým partnerem, nebo nepřímým poskytovatelem).

- Partner pracuje s novými nebo stávajícími zákazníky v těchto zemích:

    - Thajsko
    - Vietnam
    - Turecko
    - Polsko
    - Jižní Afrika
    - Indie
    - Brazílie
    - Irák
    - Myanmar
    - Jižní Súdán
    - Saúdská Arábie
    - Spojené arabské emiráty
    - Venezuela

Partneři, kteří splňují kritéria, budou muset odeslat registrační ID společnosti zákazníka (označované také jako DIČ organizace zákazníka) a telefonní číslo při příští aktualizaci nebo vytvoření předplatného pro daného zákazníka. Tito partneři můžou volitelně zadat také druhé jméno zákazníka.

Všimněte si, že při přidání registračního ID vaší společnosti byste měli použít své obchodní daňové ID, nikoli osobní ID zákazníka.

Partneři, kteří pracují s novými nebo stávajícími zákazníky v následujících zemích, už jsou připojení k předchozí verzi v listopadu 2020.

- Arménie
- Ázerbájdžán
- Bělorusko
- Maďarsko
- Kazachstán
- Kyrgyzstán
- Moldavsko
- Rusko
- Tádžikistán
- Ukrajina
- Uzbekistán

Partneři se zákazníky ve zbytku světa budou mít na konci března 2021 možnost zadat jako volitelné podrobnosti ID registrace společnosti, telefonní číslo a prostřední jméno pro zákazníky.

### <a name="next-steps"></a>Další kroky

- Podrobnější pokyny najdete v technické dokumentaci [](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) a nejčastějších dotazech ve vyhrazené kolekci partnerů.
- Připravte se na začlenění změn pomocí Partnerské centrum API a webového uživatelského prostředí. Rozhraní API nebo sdk budou k dispozici pro testování.
- Nezapomeňte odeslat další data při onboardingu nových zákazníků nebo úpravě stávajících podrobností o zákaznících.
- Pokud používáte řešení dodavatele ovládacích panelů (CPV), obraťte se na svého dodavatele CPV.

### <a name="questions"></a>Máte otázky?

Pokud máte nějaké dotazy související s ID registrace společnosti (nazývaným také "INN" nebo "TIN"). Microsoft nemůže poskytnout pokyny k daňovým záležitostem.

Pokud potřebujete podporu k operacím s Microsoftem, otevřete žádost [o služby.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a>Zobrazení nabídek a uvedení produktů pro tento měsíc na trh

### <a name="categories"></a>Kategorie

- Datum: 1. 4. 2021
- Možnosti
 
### <a name="summary"></a>Souhrn

Kalendář pro uvedení produktu na trh z dubna 2021 je nyní publikován.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Všichni partneři, kteří provádí transakce prostřednictvím Cloud Solution Provider (CSP)

### <a name="details"></a>Podrobnosti

Kalendář spuštění produktu z [](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) dubna 2021 je nyní k dispozici v galerii prostředků provozní připravenosti. Nadcházející uvedení produktů a nabídek si můžete prohlédnout tady.

### <a name="next-steps"></a>Další kroky

Zkontrolujte kalendář [spuštění produktu a](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)podělte se o informace s příslušnými účastníky ve vaší organizaci.  

### <a name="questions"></a>Máte otázky?

Pokud máte další dotazy k těmto nabídekm, podívejte se na příslušné komunity Yammeru.