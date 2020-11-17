---
title: Oznámení z listopadu 2020
description: Listopadu 2020 oznámení pro partnerské Centrum Microsoftu, včetně nových možností, propagačních akcí, nabídek, trhů nebo změn stávajících nabídek.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 11/02/2020
ms.openlocfilehash: 88d216f9e55b98f3c4818dd718c68f843c4098f0
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691295"
---
# <a name="november-2020-announcements"></a>Oznámení z listopadu 2020

Tato stránka podrobně popisuje oznámení pro partnerské Centrum Microsoftu za listopadu 2020.

2020 oznámení: [duben](2020-april.md)v  |  [May](2020-may.md)  |  [June](2020-june.md)  |  [červenci, červenec](2020-july.md),  |  [August](2020-august.md)  |  [září](2020-september.md)  |  [October](2020-October.md) | Listopadu

______________
## <a name="euefta-change-of-partner-billing-currency-for-new-commerce-offers"></a><a name="10"></a>Změna fakturační měny partnerů v EU/ESVO pro nové nabídky obchodu  

### <a name="categories"></a>Kategorie
- Datum 2020-11-17
- Možnosti

### <a name="impacted-audience"></a>Ovlivněná cílová skupina  

Partneři s podporou programu Cloud Solution Provider v oblasti EU/ESVO 

### <a name="summary"></a>Shrnutí 

V oblasti Evropské unie (EU)/European volného obchodu (ESVO) se všechny nové nabídky obchodování v programu Cloud Solution Provider použijí místo fakturačního umístění zákazníka. To znamená, že se partneři účtují společností Microsoft na základě jejich měny umístění, nikoli podle měny jejich zákazníků. To se provádí ve dvou fázích: 

- **Fáze 1: noví zákazníci, kteří si zakoupí novou nabídku Commerce v CSP**

Od ledna 2021 partneři s novými zákazníky, kteří si zakoupí nové nabídky pro obchod, se budou fakturovat za tyto nákupy v peněžních umístěních partnera. Partneři se stávajícími zákazníky, kteří si už zakoupili nové nabídky pro obchod ve zprostředkovateli CSP, se v této fázi budou dál účtovat v měně fakturačního umístění zákazníka. 

 

- **Fáze 2: stávající zákazníci, kteří si zakoupili novou nabídku pro obchodování ve zprostředkovateli CSP před lednem 2021** 

Po fázi 1 a v kalendářním roce 2021 bude Microsoft převádět účtování nových nabídek obchodu pro partnery se stávajícími zákazníky, kteří si zakoupili novou nabídku pro obchodování ve zprostředkovateli CSP před lednem 2021, od měny zákazníka až po měnu umístění partnera. Před implementací této změny se partneři budou předem informovat.  

>Značte Tato změna bude mít vliv jenom na účtovací měnu partnerů a ne na ceny za nové nabídky obchodování v CSP. 

Mezi nové nabídky pro obchod v oboru pro tuto změnu patří: předplatná Azure, která jsou součástí plánu Azure, rezervacích Azure, předplatných softwaru, trvalého softwaru a nákupů z komerčního obchodu na webu Microsoft Azure v programu Cloud Solution Provider.

### <a name="partner-benefits"></a>Výhody pro partnery  

- Tato aktualizace sníží složitost a režii při fakturaci na více měn v oblasti EU/ESVO pro nové prostředí pro obchod.  

- Partneři obdrží konsolidovanou fakturu v rámci jedné měny a nebude už dostávat fakturu pro každou měnu zákazníka na místo. 

- Výběry k pobídkám budou ve stejné měně jako fakturační měna partnera.

- Partneři budou upozorněni na složitost fakturace způsobené fakturací na více měn, což uvolní čas a prostředky, které jsou aktuálně přidruženy k sjednocování účtů. 

- Pro partnery, kteří ještě nepřijali nové nabídky obchodu, se tato změna zarovnává s předchozím modelem fakturace partnerů, takže partneři můžou snadněji přejít na nové prostředí pro obchod v rámci CSP. 

### <a name="resources"></a>Zdroje informací 

Projděte si informace o tomto tématu v [galerii operací] ( https://partner.microsoft.com/resources/collection/eu-efta-changes-collection#/ na webu Microsoft Partner.  

## <a name="api-throttling-to-partners-calling-partner-center-apis"></a><a name="9"></a>Omezování rozhraní API pro partnery, kteří volají rozhraní API partnerského centra

### <a name="categories"></a>Kategorie

- Datum 2020-11-17
- Možnosti

### <a name="summary"></a>Shrnutí

Microsoft zavádí omezování rozhraní API pro partnery, kteří volají rozhraní API partnerského centra pro zajištění jednotnějšího výkonu v daném časovém intervalu.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Natransakční partneři pomocí programu Cloud Solution Provider

### <a name="details"></a>Podrobnosti

Společnost Microsoft implementuje omezování rozhraní API v Q1 2021, aby umožňovalo jednotnější výkon v časovém intervalu pro partnery, kteří volají rozhraní API partnerského centra. Omezování omezuje počet požadavků na službu v určitém časovém rozsahu, aby nedocházelo k nadměrnému využití prostředků. Při překročení prahové hodnoty omezuje Partnerská centra všechny další požadavky od tohoto klienta po určitou dobu.  

### <a name="partner-benefits"></a>Výhody pro partnery 

Partnerské centrum je navrženo tak, aby zpracovával velký objem požadavků, ale pokud je zahlceno více požadavků několika partnery, omezování vám pomůže udržet optimální výkon a spolehlivost pro všechny partnery. Zajišťuje minimální prostoje. Díky omezení vysokého objemu požadavků můžeme zajistit konzistentní výkon pro všechny partnery. 


### <a name="apis-to-be-throttled"></a>Rozhraní API k omezení

|**Operace**|**Dokumentace k Partnerskému centru**|
|-------------------------|----------------------------------|
|{baseURL}/v1/Customers/{customer_id}/Subscriptions|[Získání všech předplatných zákazníka](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-subscriptions)|  
|{baseURL}/v1/Customers/{customer_id}/Subscriptions/{subscription_id}|[Získat předplatné podle ID](https://docs.microsoft.com/partner-center/develop/get-a-subscription-by-id) | 
|{baseURL}/v1/Customers/{customer_id}/Orders||[Získat všechny objednávky zákazníka](https://docs.microsoft.com/artner-center/develop/get-all-of-a-customer-s-orders)|  
|{baseURL}/v1/Customers/{customer_id}/Orders/{order_id}|[Získat objednávku podle ID](https://docs.microsoft.com/partner-center/develop/get-an-order-by-id)|  
|{baseURL}/v1/Customers/{customer_id}/Orders/{order_id}/provisioningstatus|[Získat stav zřizování předplatného](https://docs.microsoft.com/partner-center/develop/get-subscription-provisioning-status)|  
|{baseURL}/v1/Customers/{customer_id}/Subscriptions/{subscription_id}|[Správa objednávek a Správa předplatného](https://docs.microsoft.com/partner-center/develop/manage-orders#manage-a-subscription)| 
|{baseURL}/v1/Customers/{customer_id}/Subscriptions/{subscription_id}/addons|[Získat seznam doplňků pro předplatné](https://docs.microsoft.com/partner-center/develop/get-a-list-of-add-ons-for-a-subscription)| 
|{baseURL}/v1/Customers/{customer_id}/Subscriptions/{subscription_id}/azureEntitlements|[Získat seznam nároků na Azure pro předplatné](https://docs.microsoft.com/partner-center/develop/get-a-list-of-azure-entitlements-for-subscription)|  
|{baseURL}/v1/Customers/{customer_id}/Subscriptions/{subscription_id}/registrationstatus|[Získat stav registrace předplatného](https://docs.microsoft.com/partner-center/develop/get-subscription-registration-status)| 
|{baseURL}/v1/Customers/{Customer-tenant-ID}/Transfers|[Získat všechny přenosy zákazníka](https://docs.microsoft.com/partner-center/develop/get-subscription-registration-status)| 
|{baseURL}/v1/productUpgrades/{upgrade-id}/status|[Získat stav upgradu produktu](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-transfers)| 
|{baseURL}/v1/Customers/{Customer-ID}/Subscriptions/{Subscription-ID}/Conversions|[Získat seznam nabídek zkušebního převodu](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-transfers) 
  

Toto oznámení se zaměřuje na poskytování partnerů s včasnou informovaností o nadcházejících změnách, což jim umožní připravit se. Důrazně doporučujeme, aby se partneři seznámili s těmito rozhraními API, a zvažte použití rozhraní API protokolu aktivit pro zajištění vyšší efektivity a zabránění omezování. Další informace o této funkci najdete v tématu podrobnosti o [omezeních rozhraní API](https://docs.microsoft.com/partner-center/develop/api-throttling-guidance). 

### <a name="next-steps"></a>Další kroky

Projděte si [pokyny k omezování rozhraní API](https://docs.microsoft.com/partner-center/develop/api-throttling-guidance)a proveďte potřebné kroky. 



## <a name="409-errors-due-to-duplicate-mca-requests"></a><a name="8"></a>409 chyb způsobených duplicitními požadavky MCA

### <a name="categories"></a>Kategorie

- Datum 2020-11-16
- Možnosti

### <a name="context"></a>Kontext

- V únoru požádali partnery o podepsání smlouvy o zákaznících Microsoftu (MCuA). To bylo migrace z předchozí smlouvy Microsoft Cloud (MCA). 
- Jako součást tohoto partnera pro změny požadovali, aby partneři byli požádáni o zahrnutí parametru typu smlouvy, jak je popsáno [zde](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement).

### <a name="what-happened-next"></a>Co se stalo s následujícím:

- Ne všichni partneři zahrnuli do své implementace požadavek parametru. Microsoft vrátil pro tyto partnery tuto MCA.
- Partner pak znovu odešle žádost o podepsání zákazníkovi a znovu ji odešle společnosti Microsoft. 
- Duplikace ovlivnila schopnost Microsoftu poskytovat služby partnerům.
- V září 2020 jsme všem partnerům poslali oznámení prostřednictvím Yammeru ve více fórech a požádali, aby partneři opravili parametr. Společnost Microsoft již nemůže přijmout duplicity a obdržela 409 chyb.

>[Poznámka] Nejednalo se o novou změnu kontraktu nebo rozhraní API pro partnery.

- V říjnu jsme úzce pracovali s partnery, kteří měli nejvíce duplicitních žádostí o vyřešení problému.
- V současné době připomínáme partnerům a posílání osobních e-mailů na 10 nejčastějších pachatelů, ke kontrole jejich požadavků a k vyřešení problému, abychom vám mohli pomoci s jejich testováním.
- 10. listopadu 2020 přestaly přijímat duplicity a partneři, kteří neopravili parametry, narazili na chyby 409.
- Od té doby jsme změnili změny, aby nepřijímaly duplicity. 
- Od 14. ledna 2021 ale už nebudeme moci přijímat duplicity. Díky tomu mohou partneři docílit na své ukončení jakékoli úpravy. Již jsme dostali oznámení od partnera, který plánuje nasadit aktualizaci na 11/16, na které budeme s nimi úzce spolupracovat.
- Požadujeme, aby se partneři dostali na nás, abychom vám mohli považovat test přidáním jejich klientů do letu se změnami tak, aby se zajistilo, že jejich aktualizace řešení funguje podle očekávání.



## <a name="testing-available-partner-center-api-updates-and-user-interface-ui-enhancements-for-the-education-customer-validation-process"></a><a name="7"></a>K dispozici testování: aktualizace rozhraní API partnerského centra a vylepšení uživatelského rozhraní pro proces ověření zákazníka pro vzdělávání

### <a name="categories"></a>Kategorie

- Datum 2020-11-10
- Možnosti | Škálování & škály při zvyšování produktivity

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři prodávají akademické nabídky prostřednictvím programu Cloud Solution Provider (CSP).

### <a name="summary"></a>Shrnutí

Testování je teď k dispozici pro aktualizace rozhraní API partnerského centra a vylepšení uživatelského rozhraní pro účely procesu ověření zákazníka pro vzdělávání.

### <a name="details"></a>Podrobnosti

Microsoft běží na důvěryhodnosti. Zavázali jsme se poskytovat kompatibilní, bezpečnou a zabezpečenou metodu ověřování zákazníků pro účely transakcí akademických nabídek v programu CSP. V rámci tohoto článku zavádíme v druhém čtvrtletí tohoto fiskálního roku vylepšení rozhraní API pro partnerské centrum a uživatelské rozhraní (FY21 Q2). Tato vylepšení dostanou jasnou a srozumitelnou v rámci procesu ověřování zákazníků a také možnost zadat přesnější data, což bude zlepšit úspěšnost zákazníků při ověřování.

**Vylepšení partnerského centra**

- Nová rozhraní API pro získání a odeslání kvalifikace pro podporu přesného zadání dat a zlepšení procesu pro vzdělávání zákazníků v oblasti vzdělávání.

- Vylepšení uživatelského rozhraní pro podporu přesného zadání dat a zlepšení procesu pro vzdělávání zákazníků v oblasti vzdělávání od Microsoftu.

**Testování**

Aby bylo možné lépe pochopit rozhraní API a zadávání dat potřebné k úspěšnému ověření od zákazníka, partneři budou moci otestovat Tato vylepšení od října 2020. Brzy poskytneme další podrobnosti o přesném časování a o tom, jak se zúčastnit. Existující rozhraní API partnerského centra budou vyřazena před uplynutím FY21.2. čtvrtletí. V tuto chvíli budete muset přejít na nová rozhraní API partnerského centra.

   - Testování dostupných dat partnerských testů od 2. prosince 2020. Partneři, kteří se chtějí zúčastnit, by si stáhli příručku pro testování zákazníků z partnerského centra, kde se můžete připravit, jak se zaregistrovat a co očekávat během testovací fáze.

**Zákazníci knihoven a Museum**

Kromě těchto vylepšení vám s radostí oznamujeme, že v FY21 Q2 umožníme, abychom zákazníkům pro knihovny a Museum povolili nabídky pro akademické zákazníky a rozšíříte si zákazníky s vzděláváním, se kterými můžete vyřizovat nabídky služby Transact CSP.

Společnost Microsoft si vyhrazuje právo zkontrolovat stav každého zákazníka nebo navrženého zákazníka jako kvalifikovaného vzdělávacího uživatele. Úplné podrobnosti najdete v [požadavcích na školní potřeby vzdělávání uživatelů](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7) .

## <a name="next-steps"></a>Další kroky

Přečtěte si nové změny uživatelského rozhraní a rozhraní API partnerského centra, jakož i Průvodce testováním v [procesu ověřování zákazníků vzdělávacího centra pro vzdělávání. vylepšení shromažďování obsahu](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)

• Zaregistrujte se, abyste se mohli zúčastnit testování. (Podrobnosti najdete v [Průvodci testováním](https://partner.microsoft.com/resources/detail/partner-center-edu-testing-guide-pdf) .) 

• Ujistěte se, že vaše organizace je obeznámená s [požadavky školního uživatele na vzdělávání](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7). 

• Sdílejte tyto informace s příslušnými týmy v rámci vaší organizace spolu s prodejci, aby jim pomohli připravit se na tyto změny.



## <a name="expanding-commercial-licensing-partner-content-on-the-operations-readiness-gallery"></a><a name="6"></a>Rozšiřování obsahu komerčního licenčního partnera v galerii připravenost k provozu

### <a name="categories"></a>Kategorie

- Datum: 2020-11-5
- Možnosti

### <a name="summary"></a>Shrnutí

Od listopadu 5 2020 budou k dispozici komerční obsah partnerského oddělení z partnerské univerzity, a to i v galerii připravenost k provozu.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Komerční partneři

### <a name="details"></a>Podrobnosti

Od 5. listopadu 2020 bude k dispozici komerční obsah partnerského oddělení z partnerské univerzity, který bude dostupný i v galerii připravenost k provozu. Tím se už stávající provozní a komerční licenční partner spustí obsah v galerii připravenost k provozu s naším dlouhodobě komerčním partnerem licencování od partnerského studia. Díky tomu budou mít partneři pružnější možnosti připravenosti. Do galerie připravenost k operacím byly přidány následující kolekce:

- [Microsoft Azure – nabídky a licencování](https://partner.microsoft.com/resources/collection/microsoft-azure-offers-and-licensing#/)
- [Komerční licencování – volání Spotlightu pro CSP](https://partner.microsoft.com/resources/collection/commercial-licensing-csp-spotlight-call#/)
- [Komerční licencování – volání aktualizací licencování](https://partner.microsoft.com/resources/collection/commercial-licensing-licensing-updates-call#/)

### <a name="next-steps"></a>Další kroky

Tyto informace Sdílejte se všemi odpovídajícími kontakty ve vaší organizaci.

________________

## <a name="microsoft-teams-rooms-premium-sku-launch"></a><a name="5"></a>Microsoft Teams Rooms úrovně Premium – spuštění SKU

### <a name="categories"></a>Kategorie

- Datum: 2020-11-3
- Nabídky/trhy

### <a name="summary"></a>Shrnutí

Microsoft Teams je teď dostupný v programu Cloud Solution Provider (CSP) pro týmy Microsoft.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Všechny partnery, kteří se docházejí prostřednictvím programu Cloud Solution Provider (CSP)

### <a name="details"></a>Podrobnosti

Nové týmy Microsoft Teams jsou teď dostupné pro vaše zákazníky, kteří si kupují poskytovatele CSP za USD50 na zařízení za měsíc. SKU Microsoft Teams je alternativou k Microsoft Teams místnosti Standard SKU (dříve označované jako licence na schůzku). Tato SKU obsahuje všechno ve standardní nabídce, jako jsou třeba licence pro Microsoft teams, Online Skype pro firmy a správu Intune. Nabídka taky umožňuje telefonnímu systému – nutnému pro integraci veřejné telefonní sítě (PSTN) a zvukové konference, kde je k dispozici. 

Díky nabídce Premium mají zákazníci přístup k nově vydaným verzím Microsoft Teams místností spravované služby, kde odborníci zpracovávají správu a operace pro místnosti pro schůzky jménem zákazníka. Tato cloudová služba pro správu a sledování IT zajišťuje, aby týmy Microsoftu místnosti zařízení a jejich periferních zařízení v aktuálním stavu. Také se aktivně monitorují a spravují a udržují prostředí optimalizované pro skvělou práci v místnosti.

#### <a name="released-at-launch"></a>Vydaná při spuštění

   |****|**Microsoft Teams Rooms úrovně Standard USD15 za měsíc**|**Microsoft Teams Rooms Premium USD50 Device za měsíc**|
   |-------------------|:------|:------|
   |Skype pro firmy|Yes| |
   |Microsoft Teams|Yes|Yes|
   |Telefonní systém|Yes|Yes|
   |Zvukové konference|Yes|Yes|
   |Microsoft Intune|Yes|Yes|
   | |Microsoft Teams Rooms Standard USD15 na zařízení za měsíc|Microsoft Teams Rooms Premium USD50 na zařízení za měsíc|
   |Microsoft Teams místností spravované služby| |Yes|
   |Celosvětová dostupnost|Yes|Na vybraných trzích|

#### <a name="microsoft-teams-rooms-managed-services"></a>Microsoft Teams místností spravované služby

- Proaktivní Správa: zcela nepřetržitou správu vašich systémů místností, včetně oprav, správy konfigurací a dalších.
• Monitorování a analýza hlavní příčiny v reálném čase: monitorování a zjišťování s orchestrací reakce na správu incidentů, kterou zajišťuje Microsoft v koordinaci s zákazníkem v případě potřeby. Mobilní aplikace vám umožní udržet výstrahy na cestách.
- Spravované aktualizace: Správa a doručování aktualizací aplikací, Windows KB a firmwaru.
- Ochrana před hrozbami zabezpečení: Ochrana před internetovými útoky pomocí rozšířené ochrany před internetovými útoky v programu Microsoft Defender
- Zákaznická podpora: podpora lístků zcela nepřetržitou prostřednictvím našeho vyhrazeného provozního centra služeb s asistencí pro jiné než automatizované případy. Podrobné řízení přístupu na základě rolí.
- Přehledy a doporučení: agregované přehledy pro zákazníky a sestavy o stavu místnosti, inventáři, používání, online schůzkách a trendech incidentů.

#### <a name="offer-details"></a>Podrobnosti nabídky

   |**Název nabídky**|**ID nabídky**|**ID materiálu**|
   |-------------------|:------|:------|
   |Týmy na místnosti úrovně Premium|5db9aa31-f039-4740-b122-a33514e4c492|6XB-00007|
   |Týmy v místnostech Premium (USA a může)|03070f91-cc77-4c2e-b269-4a214b3698ab|6XB-00008|
   |Týmy – místnosti Premium pro vyučující|d0c9a9a9-c9b6-41d7-9148-b60115c36c95|6Y5-00005|

### <a name="next-steps"></a>Další kroky

- Seznamte se s novou nabídkou a její geografickou dostupností najdete [v nejčastějších dotazech.]()
- Seznámení s novou nabídkou a její geografickou dostupností 
- Přečtěte si další informace o místnostech Microsoftu a souvisejících nabídkách na [týmových místnostech Microsoftu](https://rooms.microsoft.com/).
- Pomocí [Průvodce týmy pro týmy](https://aka.ms/teamscallingmeetingsguide) můžete vyvinout svůj postup s týmy pro setkání a vytvořit nabídku, která je připravená pro spoluprodej.
- Přečtěte si [Nejčastější dotazy k místnostem Microsoft Teams](https://aka.ms/PartnerMTRFAQ) , kde najdete další informace o řešení a službách produktu. 
- Tyto informace se dají sdílet se všemi příslušnými kontakty ve vaší organizaci a porozumět příležitostem přeprodat a vzájemným prodejcům.

________________

## <a name="new-microsoft-teams-advanced-communications-skus-for-government-community-cloud-gcc-coming-soon"></a><a name="4"></a>Nové Microsoft Teams Advanced Communications pro Cloud Community (RSZ) již brzy

### <a name="categories"></a>Kategorie

- Datum: 2020-11-2
- Nabídky/trhy

### <a name="summary"></a>Shrnutí

Nové skladové položky doplňku pro pokročilou komunikaci pro Microsoft Teams v RSZ budou k dispozici od 1. prosince 2020.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Všechny partnery, kteří se docházejí prostřednictvím programu Cloud Solution Provider (CSP)

### <a name="details"></a>Podrobnosti

Nový doplněk pro pokročilou komunikaci pro Microsoft Teams v RSZ je teď k dispozici na USD12 na uživatele měsíčně. SKU doplňku se dají koupit na jakékoli jiné Microsoft 365 sady, která obsahuje Microsoft Teams. Pokročilá komunikace poskytuje novou sadu funkcí pro velké schůzky, zásady komunikace, integrace a rozšířené nástroje pro správu IT. 

#### <a name="offer-details"></a>Podrobnosti nabídky

   |**Název nabídky**|**ID nabídky**|**ID materiálu**|
   |-------------------|:------|:------|
   |Pokročilá komunikace pro RSZ|56fe76f5-f4ba-4fac-9561-d0daf59b01a1|7FB-00003|

#### <a name="frequently-asked-questions"></a>Nejčastější dotazy 

**Co je pokročilá komunikace?** Tento nový doplněk Microsoft Teams umožňuje zákazníkům dále zvyšovat možnosti komunikace. Dá se koupit na Microsoft 365 SKU, ke kterému se přihlásí.

**Kolik to stojí?** Komerční ERP je USD12 na uživatele a měsíc.

**Kteří zákazníci si doplněk můžou koupit?** Zákazníci v rámci RSZ si můžou doplněk koupit.

**Jak se dá koupit?** Tento doplněk můžete koupit prostřednictvím smlouva Enterprise, smlouva Enterprise předplatného, registrace pro vzdělávací řešení, CSP nebo webu Direct.

**Kde se dá prodávat?** Dá se prodávat na trzích USA.

**Jaké jsou požadavky?** Tento doplněk můžou mít všechny Microsoft 365 nebo sady Office 365, které obsahují Microsoft Teams.

### <a name="next-steps"></a>Další kroky

Tyto informace se dají sdílet s příslušnými kontakty ve vaší organizaci a porozumět příležitostem přeprodat a vzájemným prodejcům. Projděte si část prostředky v [příručce Teams partner](https://aka.ms/teamscallingmeetingsguide).

________________

## <a name="dynamics-365-recently-launched-and-upcoming-new-offers-and-products"></a><a name="3"></a>Dynamics 365: Nedávno spuštěné a nadcházející nové nabídky a produkty

### <a name="categories"></a>Kategorie

- Datum: 2020-11-2
- Nabídky/trhy

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Přímí poskytovatelé, nepřímá poskytovatelé a nepřímí prodejci

### <a name="details"></a>Podrobnosti

#### <a name="new-offers"></a>Nové nabídky

Od 1. listopadu 2020 nabízí Microsoft Dynamics 365 operace projektu a odebrali jsme pro komerční zákazníky Dynamics 365 Project Service Automation (PSA). Tato komunikace poskytuje další informace týkající se mapování duálních práv na používání z tohoto spuštění a nového nezávislého výrobce softwaru (ISV) Embedded.

#### <a name="project-operations-isv-embed-offers"></a>Nabídky operací s projektem ISV pro vložení

Od 1. listopadu 2020 společnost Microsoft vydávala tři další 36 nabídky za za měsíc pro produkt Dynamics 365 pro projektové operace pro zákazníky poskytovatele Cloud Solution Provider (CSP). Podrobnosti o SKU najdete v [dokumentu Dynamics CSP Offers-November 2020 Excel v dokumentu aplikace](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-november-xls) Project – karta operace projektu.

#### <a name="project-operations-dual-use-rights-mapping"></a>Operace projektu – mapování oprávnění pro duální použití

Informace o právech pro duální použití v Dynamics 365 pro místní mapování pro projektové operace nabídky najdete v následující tabulce:

   |**Nabídka operací D365**|**Mapování místních práv na používání duálního použití D365**|
   |-------------------|:------|
   |Nabídka operací D365|Mapování místních práv na používání duálního použití D365|
   |Operace projektu D365|D365 for Operations, on-Prem (AX Server) s použitím skladové položky SKU pro Dyn365 projektu (109108477)|
   |Připojení operací projektu D365|D365 for Operations, on-Prem (AX Server) s použitím skladové položky SKU pro Dyn365 projektu (109108477)|
   |D365 finance s operacemi projektu|D365 for Operations, on-Prem (AX Server) s použitím skladové položky SKU pro Dyn365 projektu (109108477)|
   |D365 finance připojit k projektovým operacím|D365 for Operations, on-Prem (AX Server) s použitím skladové položky SKU pro Dyn365 projektu (109108477)|
   |D365 Unified Operations – aktivita s operacemi projektu|D365 for Operations, on-Prem (AX Server) s použitím skladové položky SKU pro Dyn365 projektu (109108477)|

#### <a name="previously-announced"></a>Dřív oznámeno

Od 1. listopadu 2020 společnost Microsoft zveřejnila následující nové a aktualizované nabídky produktů Dynamics 365 a Power Platform pro CSP:

- Dynamics 365 Customer Voice USL 

Podrobnosti o ID nabídky najdete v [dokumentu Dynamics CSP Offers-November 2020 Excelu v dokumentu aplikace](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-november-2020-xls) Project – karta operace projektu.

Další zdroje najdete na domovské stránce hlasu pro zákazníky Microsoft Dynamics 365.

### <a name="next-steps"></a>Další kroky

Tyto informace sdílejte s příslušnými lidmi ve vaší organizaci.

________________

## <a name="introducing-microsoft-365-business-voice-for-nonprofit-organizations"></a><a name="2"></a>Představujeme Microsoft 365 Business hlas pro neziskové organizace

### <a name="categories"></a>Kategorie

- Datum: 2020-11-2
- Nabídky/trhy

### <a name="summary"></a>Shrnutí

Od listopadu 1 2020 společnost Microsoft zavedla nové SKU pro Microsoft 365 Business hlas pro neziskové organizace.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Přímí poskytovatelé, nepřímá poskytovatelé a nepřímí prodejci

### <a name="details"></a>Podrobnosti

Od 1. listopadu 2020 společnost Microsoft zavedla nové SKU pro obchodní telefony. Úplná sada je dostupná v Kanadě, Spojeném království a USA. Obchodní telefon bez volání plánu bude k dispozici na všech ostatních trzích. 

Microsoft 365 Business Voice je cloudový telefonní systém pro malé a střední podniky, které jsou součástí sady Office 365. Přidání obchodního hlasu do předplatného Office 365 zákazníka přináší řešení pro komunikaci a spolupráci typu "vše v jednom" s voláním, chatem a schůzkami v jediné aplikaci, Microsoft Teams.

Podrobnosti o cenách najdete v ceníku.

Microsoft 365 Business hlas můžete přidat do následujících předplatných až 300 uživatelů:

- Office 365: Business Essentials, Business Premium, a1, E1, a3 a E3
- Microsoft 365: Business, a3 a E3


### <a name="next-steps"></a>Další kroky

- Seznamte se s příslušnými kontakty ve vaší organizaci a sdílejte informace v seznamu ceny verze Preview. 
- Projděte si všechny materiály připravenosti v galerii prostředků aktualizace programu poskytovatele Cloud Solution: [představujeme Microsoft 365 Business hlas pro malé a střední firmy](https://partner.microsoft.com/resources/collection/m365-voice-smb#/). 

________________

## <a name="cloud-solution-provider-csp-promo-for-microsoft-365-business-voice-is-now-available"></a><a name="1"></a>K dispozici je teď propagační akce poskytovatele Cloud Solution Provider (CSP) pro Microsoft 365 Business Voice

### <a name="categories"></a>Kategorie

- Datum: 2020-11-2
- Nabídky/trhy

### <a name="summary"></a>Shrnutí

Zlevněné ceny pro nové a obnovení předplatných Microsoft 365 Business hlasu pomocí plánu volání a Microsoft 365 Business hlasu bez volání plánu.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Všichni partneři s podporou v rámci programu CSP

### <a name="details"></a>Podrobnosti

Od 1. listopadu 2020 do 30. dubna 2021, nového a obnovování předplatných Microsoft 365 Business hlasu s voláním plánu a Microsoft 365 Business hlasový hovor bez volání plánu se účtují za zlevněné ceny. Microsoft 365 Business hlas s plánem volání podléhá 25% slevám po dobu 12 měsíců a Microsoft 365 Business hlasový hovor bez volání plánu podléhá 33% slevě po dobu 12 měsíců. 

#### <a name="offer-details"></a>Podrobnosti nabídky

   |**Název nabídky**|**ID nabídky**|**ID materiálu**|
   |-------------------|:------|:------|
   |Propagační akce při přijetí Microsoft 365 Business řeči|e7d1d0fa-b769-45c7-aaea-c3e6f7402691|PZX-00006|
   |Propagační akce při přijetí Microsoft 365 Business řeči|ef3ff6bb-a288-4a56-9204-97b37ff9a0b8|PZW-00019|
   |Propagační akce při přijetí Microsoft 365 Business hlasu (US)|4244aed3-90ae-4754-8dc8-37f2e8d84e85|PZW-00020|
   |Microsoft 365 Business hlas (bez volání plánu) – propagační akce|b71df433-6fd9-4549-886d-577f7aa06070|PZY-00019|
   |Microsoft 365 Business hlas (bez volání plánu) – propagační akce|4ba4d580-4902-42b0-8411-a27358dd5405|PZY-00016|
   |Microsoft 365 Business hlas (bez volání plánu) – propagační akce|bbfd896b-e3d4-45ba-9319-14104d400069|PZY-00018|
   |Microsoft 365 Business hlas (bez volání plánu) pro propagační přijetí v USA|9b05d0b7-cfb4-42f1-9cc3-f698dba2838e|PZY-00017|

Tyto propagační akce mají vliv na tyto zákazníky:

- Klienti s čistým novým zákazníkem
- Stávající vzdálení klienti, kteří nemají aktivní nebo nedávno zrušené předplatné (během posledních 30 dnů), mají licenci na podnikovou nebo bezplatnou licenci na CSP, web Direct nebo jiný komerční kanál Microsoftu.

#### <a name="additional-resources"></a>Další zdroje informací

- Další informace o obchodním hlasu najdete na [stránce Microsoft 365 Business hlasového partnera](https://www.microsoft.com/microsoft-365/partners/businessvoice) . 
- Přečtěte si další informace o této propagačních DOTAZech v souvisejícím [partnerovi](https://www.microsoft.com/microsoft-365/partners/resources/faq-business-voice-audio-conferencing-promo).

### <a name="next-steps"></a>Další kroky

- Seznamte se s těmito schůzkami a zavoláním propagačních příležitostí a sdílejte tyto informace se všemi příslušnými kontakty ve vaší organizaci.
- Tyto propagační akce zahrňte do prodejních pohybů v Microsoft 365.
- Dodávejte zákazníkům povědomí o hodnotě přidávání obchodních hlasů do týmů. 

________________
