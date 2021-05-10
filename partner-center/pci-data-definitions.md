---
title: Definice dat Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dokument obsahuje seznam různých sestav a jejich definicí dat, které si můžete stáhnout ze stránky sestavy stažení přehledů.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21be5b22c453174fcb66e9409d6e26dad8e25c6b
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686343"
---
# <a name="export--data-definitions"></a>Export – definice dat 

**Příslušné role** 

- Prohlížeč sestav
- Prohlížeč sestav Executive

## <a name="introduction"></a>Úvod 

Pomocí centra pro stažení sestav na řídicím panelu Insights můžete exportovat nezpracované datové sady. 

Různé sestavy, které si můžete stáhnout spolu s definicemi jejich dat, jsou uvedené v následujících tabulkách: 

### <a name="partner-profile-report"></a>**Sestava profil partnera**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| MPNId | Identifikátor Microsoft Partner Network (MPN) | 
| PartnerName | Název partnera | 
| PGA_MPNId | Identifikátor účtu MPN globálního účtu partnera | 
| PGA_PartnerName | Název globálního účtu partnera | 
| City (Město) | Město, kde se nachází partner | 
| Země | Umístění země partnera | 
| HierarchyLevel | Označuje, jestli se jedná o globální ID MPN, nebo ID MPN umístění. | 

### <a name="customer-details-report"></a>**Sestava podrobností o zákazníkovi**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerName | Jméno zákazníka | 
| CustomerTenantId | Identifikátor tenanta zákazníka | 
| CustomerTpid | Identifikátor nadřazeného zákazníka | 
| CustomerSegment | Segment zákazníka | 
| CustomerMarket | Geografický trh zákazníka | 
| Stav zákazníka | Stav zákazníka (aktivní nebo neaktivní) | 
| Produkt | Produkt prodaný zákazníkovi podle MPN: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI nebo Microsoft Azure | 
| SKU | SKU produktu | 
| Month (Měsíc) | Měsíc, za který se hlásí využití a výnosy | 
| ID MPN | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| PartnerLocation | Zeměpisné umístění partnera | 
| PartnerAttributionType | Typ přidělení partnera | 
| SalesChannel | Prodejní kanál | 
| AvailableSeats | Dostupná místa | 
| RevenueUSD | Tržby v amerických dolarech | 

### <a name="reseller-performance-report"></a>**Sestava o výkonu prodejce**

> [!Note]
> Data o výnosech a ACR jsou k dispozici pouze uživatelům, kteří jsou správci sestav od manažera.

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ResellerMPNid | Identifikátor Microsoft Partner Network prodejce | 
| ResellerName | Jméno prodejce | 
| ResellerMarket | Prodejce země na trhu | 
| IndirectProviderMPNId | Identifikátor Microsoft Partner Network nepřímého zprostředkovatele | 
| IndirectProviderName | Název nepřímého zprostředkovatele | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití a výnosy | 
| Produkt | Název produktu | 
| ID předplatného | Identifikátor předplatného | 
| AvailableSeats | Počet dostupných licencí | 
| AssignedSeats | Počet přiřazených licencí | 
| BilledRevenue | Fakturované výnosy v amerických dolarech | 
| CustomerName | Jméno zákazníka | 
| CustomerTPid | Identifikátor nadřazeného zákazníka | 
| CustomerSegment | Segment zákazníka | 
| CustomerMarket | Geografický trh zákazníka | 
| ResellerStatus | Stav prodejce | 

### <a name="subscription-details-report"></a>**Sestava podrobností o předplatném**

>[!Note]
>Údaje o výnosech a ACR jsou k dispozici pouze uživatelům, kteří jsou diváky sestav vedení.

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| SubscriptionId | Identifikátor GUID předplatného | 
| SubscriptionStartDate | Počáteční datum předplatného | 
| SubscriptionEndDate | Datum ukončení předplatného | 
| SubscriptionState | Stav předplatného (aktivní nebo změněný) | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití a výnosy | 
| IsAutoRenew | Indikuje, jestli se předplatné má obnovit (Ano nebo ne). | 
| CustomerName | Jméno zákazníka | 
| CustomerTenantId | Identifikátor GUID zákazníka | 
| CustomerTpid | Hlavní nadřazený identifikátor zákazníka | 
| CustomerSegment | Tržní segment zákazníka | 
| CustomerMarket | Zeměpisný trh zákazníka | 
| Produkt | Produkt prodávaný partnerem pro zákazníky | 
| SKU | SKU produktu | 
| ID MPN | Microsoft Partner Network ID partnera | 
| PartnerName | Název partnera | 
| PartnerLocation | Zeměpisné umístění partnera | 
| PartnerAttributionType | Typ atribuce pro předplatné | 
| SalesChannel | Kanál prodeje – Přímý, CSP (Cloud Solution Provider) a tak dále | 
| AvailableSeats | Aktuální dostupná místa | 
| Revenue (Výnosy) | Revenue in US dollars | 
| ID registrace | ID registrace předplatného | 

### <a name="azure-usage-report"></a>**Sestava využití Azure**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| SubscriptionId | GUID předplatného | 
| Datum_zahájení_předplatného | Datum začátku předplatného | 
| SubscriptionEndDate | Datum konce předplatného | 
| SubscriptionState | Aktuální stav předplatného (otevřené, uzavřené, aktivní nebo v období odkladu) | 
| Month (Měsíc) | Datum agregované podle měsíce | 
| ServiceName | Název služby Azure | 
| MeterCategory | Název kategorie měřiče | 
| UsageUnits | Počet jednotek, které se používají během fakturačního cyklu. | 
| CustomerName | Jméno zákazníka | 
| CustomerTenantId | ID tenanta zákazníka | 
| CustomerTpid | Hlavní ID nadřazeného zákazníka | 
| CustomerSegment | Segment zákazníka | 
| CustomerMarket | Zeměpisný trh zákazníka | 
| MPNId | ID Microsoft Partner Network zákazníka | 
| PartnerName | Název partnera | 
| PartnerLocation | Zeměpisná poloha země partnera | 
| PartnerAttributionType | Typ přidělení partnera | 
| SalesChannel | Kanál prodeje (přímý/CSP, nepřímý/CSP, přímý atd.) | 
| ACR_USD | Azure spotřebované tržby (ACR) v amerických dolarech | 
| ID registrace | ID registrace předplatného Azure | 

### <a name="office-365-license-usage-report"></a>**Sestava využití licencí Office 365**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenanta zákazníka | 
| CustomerTpid | Hlavní ID nadřazeného zákazníka | 
| Úloha úlohy | Skype pro firmy, týmy, Exchange Online | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití | 
| PaidAvailableUnits | Počet placených jednotek k dispozici | 
| MonthlyActiveUsers | Počet aktivních uživatelů za měsíc | 
| CustomerName | Jméno zákazníka | 
| CustomerMarket | Zeměpisná poloha země na trhu zákazníka | 
| CustomerSegment | Segment zákazníka | 
| MPNId | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| PartnerLocation | Zeměpisné umístění partnera | 
| PartnerAttributionType | Typ přidělení partnera | 

### <a name="enterprise-mobility-license-usage-report"></a>**Sestava využití licencí Enterprise mobility**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenanta zákazníka | 
| CustomerTpid | Hlavní ID nadřazeného zákazníka | 
| Úloha úlohy | Název úlohy Enterprise Mobility + Security (EMS) | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití | 
| PaidAvailableUnits | Počet placených jednotek k dispozici | 
| MonthlyActiveUsers | Počet aktivních uživatelů za měsíc | 
| CustomerName | Jméno zákazníka | 
| CustomerMarket | Zeměpisná poloha země na trhu zákazníka | 
| CustomerSegment | Segment zákazníka | 
| MPNId | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| PartnerLocation | Zeměpisné umístění partnera | 
| PartnerAttributionType | Typ přidělení partnera | 

### <a name="dynamics-365-license-usage-report"></a>**Sestava využití licencí Dynamics 365**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| SubscriptionId | GUID předplatného | 
| Datum_zahájení_předplatného | Počáteční datum odběru | 
| Datum ukončení předplatného | Koncové datum předplatného | 
| Stav předplatného | Stav předplatného | 
| Month (Měsíc) | Měsíc, pro který se hlásí využití | 
| RevSumDivisionName | Název dělení rev sum | 
| RevSumCategoryName | Název kategorie součetu revize | 
| SKU | SKU produktu | 
| ID SKU | ID SKU produktu | 
| FreeVsPaidSKU | Určuje, jestli se jedná o bezplatnou nebo placenou SKU. | 
| SalesModel (Model prodeje) | Prodejní kanál, který se používá k prodeji předplatného | 
| Model DetailedSalesModel | Podrobný prodejní model předplatného | 
| CustomerName | Jméno zákazníka | 
| CustomerTenantId | Identifikátor GUID tenanta zákazníka | 
| CustomerTpid | Hlavní nadřazený identifikátor zákazníka | 
| CustomerSegment | Tržní segment zákazníka | 
| CustomerMarket | Zeměpisný trh zákazníka | 
| MPNId | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| PartnerLocation | Zeměpisná poloha země partnera | 
| PartnerAttachType | Typ přidělení pro předplatné | 
| AvailableSeats | Aktuální dostupné místo | 
| AssignedSeats | Aktuální přiřazené místo | 
| ActiveSeats | Aktuální aktivní verze licencí | 
| NasazeníOpportunity | Aktuální příležitost nasazení | 
| AktivníusagePercent | Procento aktuálního aktivního využití | 

### <a name="power-bi-license-usage-report"></a>**Power BI využití licencí**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| SubscriptionId | GUID předplatného | 
| Datum_zahájení_předplatného | Počáteční datum odběru | 
| Datum ukončení předplatného | Koncové datum předplatného | 
| Stav předplatného | Stav předplatného (aktivní, neaktivní nebo v období odkladu) | 
| Month (Měsíc) | Datum agregované podle měsíce | 
| SKU | SKU produktu | 
| SKUId | ID SKU produktu | 
| FreeVsPaidSKU | Neplacený nebo placený rozdíl SKU | 
| SalesModel | Prodejní model, který se používá k prodeji předplatného | 
| DetailedSalesModel | Podrobný prodejní model předplatného | 
| CustomerName | Jméno zákazníka | 
| CustomerTenantId | Identifikátor GUID tenanta zákazníka | 
| CustomerTpid | Identifikátor nejvyšší nadřazené položky zákazníka | 
| CustomerSegment | Tržní segment zákazníka | 
| CustomerMarket | Zeměpisný trh zákazníka | 
| MPNId | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| PartnerLocation | Zeměpisná poloha země partnera | 
| PartnerAttachType | Typ přidělení pro předplatné | 
| AvailableSeats | Aktuální dostupné verze licencí | 
| AssignedSeats | Aktuálně přiřazené licencí | 
| ActiveSeats | Aktuální aktivní verze licencí | 
| NasazeníOpportunity | Aktuální příležitost nasazení | 
| AktivníusagePercent | Procento aktuálního aktivního využití | 

### <a name="teams-meetings-and-calls-report"></a>**Sestavy schůzek a volání Teams**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenanta zákazníka | 
| CustomerTpid | Identifikátor nadřazeného zákazníka | 
| Month (Měsíc) | Měsíc, pro který se hlásí využití | 
| Dílčí část | Dílčí část, pro kterou se hlásí využití (schůzky, hovory nebo telefonní systémy) | 
| Počet schůzek | Počet schůzek | 
| Doba trvání schůzky | Celková doba trvání schůzky v hodinách | 

### <a name="teams-monthly-usage-report"></a>**Sestava měsíčního využití týmů**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenanta zákazníka | 
| CustomerTpid | Identifikátor nejvyšší nadřazené položky zákazníka | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití | 
| Podúlohy | Podúlohy, pro které se nahlásí využití (schůzky, hovory nebo telefonní systémy) | 
| Uživatelé klasické pracovní plochy | Počet uživatelů, kteří používají týmy na ploše | 
| Mobilní uživatele | Počet uživatelů, kteří používají týmy na mobilních zařízeních | 
| Webové uživatele | Počet uživatelů, kteří používají týmy na webu | 
| AllUpParticipants | Počet jedinečných uživatelů týmů v měsíci | 

### <a name="teams-usage-3p-apps-report"></a>**Sestava využití 3P aplikací týmů**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenanta zákazníka | 
| CustomerTpid | Hlavní ID nadřazeného zákazníka | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití | 
| Název aplikace 3P | Název aplikace Teams | 
| Počet uživatelů | Počet uživatelů pro aplikaci | 


### <a name="training-details-report"></a>**Sestava podrobností o školení**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| TrainingActivityId | Identifikátor školení | 
| TrainingTitle | Název školení | 
| TrainingType | Typ školení (certifikace nebo zkouška) | 
| IndividualFirstName | Křestní jméno zákazníka | 
| IndividualLastName | Příjmení zákazníka | 
| E-mail | Osobní e-mailové ID zákazníka | 
| CorpEmail | ID e-mailu office zákazníka | 
| TrainingCompletionDate | Datum dokončení trénování | 
| Month (Měsíc) | Měsíc, pro který jsou data hlášena | 
| IcMCP | Určuje, jestli je uživatel odborníkem na certifikaci Microsoft Certified Professional (MCP). | 
| MCPID | ID MCP uživatele | 
| ID MPN | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| PartnerCityLocation | Zeměpisné umístění města partnera | 
| PartnerCountryLocation | Zeměpisné umístění země partnera | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn sestavy**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| Uživatelské jméno | Jméno uživatele | 
| UserId | IDENTIFIKÁTOR GUID uživatele | 
| Procvičení | Název školení | 
| TrainingType | Typ školení (modul nebo vzdělávací cesta) | 
| Produkty | Produkt, na který se vztahuje modul učení | 
| Role | Příslušné role školení | 
| CompletionDate | Datum dokončení školení | 
| MPNId | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| Země | Zeměpisná poloha země partnera | 

### <a name="competency-summary-and-history-report"></a>**Souhrn kompetencí a sestava historie**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CompetencyName | Název kompetence | 
| CompetencyLevel | Úroveň kompetence (zlatá nebo stříbrná) | 
| CompetencyStatus | Aktuální stav kompetence (aktivní, neaktivní nebo v období odkladu) | 
| Datum zahájení kompetencí | Počáteční datum kompetence | 
| Datum ukončení kompetencí | Koncové datum kompetence | 

### <a name="competency-performance-report"></a>**Sestava výkonu kompetencí**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| Název kompetence | Název kompetence | 
| CompetencyAttainmentOptionName | Název možnosti dosažené kompetence | 
| Month (Měsíc) | Měsíc, pro který se metriky hlásí | 
| MetricName | Název metriky, která je relevantní pro kompetenci | 
| MetricMonthlyContribution | Měsíční příspěvek metriky | 
| TTMAggregate | Agregovaná metrika za posledních 12 měsíců | 
| AnniversaryYearAggregate | Agregovaná metrika pro aktuální rok výročí | 
| GoldThreshold | Požadavek na výkon pro splnění kompetence Gold Competency | 
| SilverThreshold | Požadavek na výkon pro uspokojení stříbrné kompetence | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Sestava o proMicrosoft 365ch properch v cloudu**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ID MPN | ID Microsoft Partner Network | 
| Název partnera | Název partnera | 
| ID zákazníka | Číslo identifikátoru zákazníka | 
| DUNS číslo | Telefonické připojení & Bradstreet (D&B) číslo zákazníka, u kterého se má vyhodnocovat hodnocení Proper | 
| Account Name | Název účtu | 
| Doména | Doména účtu | 
| Velikost organizace | Velikost organizace | 
| Obor | Odvětví, do kterého organizace patří | 
| Svisle | Svislá část zákazníka, u kterého se skóre v rámci PROPER identifikovali podle identifikace od Microsoftu, D&B a dalších oborových standardů | 
| Plošný | Zeměpisná oblast umístění | 
| Pobočka | Dceřiná společnost zákazníka, u kterého se má skóre na Proper | 
| Sales Territory (Prodejní oblast) | Prodejní teritorium zákazníka, u kterého se provádí hodnocení Proper | 
| City (Město) | Zeměpisná poloha města organizace | 
| Stav | Zeměpisné umístění organizace | 
| PSČ | PSČ organizace | 
| Země | Zeměpisné umístění země organizace | 
| Segment | Segment trhu | 
| Dílčí segment | Dílčí podsegment trhu | 
| Souhrn typů SMC | Typ SMC | 
| Nejspravované – výpočetní základ | Nejspravovaná zákazníci – výpočetní prostředky | 
| Nejspravované – uživatelská základna | Nejspravovaná zákazníci – uživatel | 
| IsNonProfit | Určuje, jestli je organizace nezisková (Ano nebo Ne). | 
| Povolení vzdálené práce – cílový Exchange Online | Zákazníci, kteří mají aktivní předplatné Exchange Online, prodávat Microsoft 365 | 
| Povolení vzdálené práce – místní získání (aktuální verze) s licencí Cloud Ascent – +10 licencí | Zákazník, který má aktuálního místního klienta Office nebo Windows To znamená, že verze klienta je novější než verze EOL (End of Life). Zákazník má 10 nebo více licencí. Zákazník, který má skóre sklonu. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní akvizici (aktuální verze) s licencemi pro PROPER v cloudu – <10 | Zákazník, který má stávajícího místního Office nebo klienta Windows (tj. verze novější než konce řádku). Zákazník má méně než 10 licencí. Zákazník, který má skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní pořízení (aktuální verze) bez licencí PROPER v cloudu – + 10 | Zákazník, který má stávajícího místního Office nebo klienta Windows (tj. verze novější než konce řádku). Zákazník má 10 nebo více licencí. Zákazník nemá skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní pořízení (aktuální verze) bez <10 licencí v cloudu | Zákazník, který má stávajícího místního Office nebo klienta Windows (tj. verze novější než konce řádku). Zákazník má méně než 10 licencí. Zákazník nemá skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní akvizici (konce řádku verzi) s licencemi pro procházím cloudovým properm – + 10 | Zákazník, který má konce řádku místního Office nebo klienta Windows (to znamená, že konce řádku verze nebo starší). Zákazník má 10 nebo více licencí. Zákazník má skóre proper. Partner by měl cílit na převod na Microsoft 365. | 
| Povolení vzdálené práce – místní získání (verze EOL) s licencí Cloud Ascent – <10 licencí | Zákazník, který má místního klienta Office nebo Windows EOL (tj. verzi EOL nebo starší). Zákazník má méně než 10 licencí. Zákazník má skóre sklonu. Partner by měl cílit na převod na Microsoft 365. | 
| Povolení vzdálené práce – místní získání (verze EOL) bez licence Cloud Ascent – +10 licencí | Zákazník, který má aktuálního místního klienta Office nebo Windows (tj. verzi EOL nebo starší). Zákazník má 10 nebo více licencí. Zákazník nemá skóre sklonu. Partner by měl cílit na převod na Microsoft 365. | 
| Povolení vzdálené práce – místní získání (verze EOL) bez licence Cloud Ascent – <10 licencí | Zákazník, který má aktuálního místního klienta Office nebo Windows (tj. verzi EOL nebo starší). Zákazník má méně než 10 licencí. Zákazník nemá skóre sklonu. Partner by měl cílit na převod na Microsoft 365. | 
| Povolení práce na dálku – potenciální potenciální zákazník s vysokou Microsoft 365 (Act NowithEvaluate) | Potenciální zákazník s vysokou Microsoft 365 | 
| Povolit práci na dálku – konkurovat (Zoom) s Microsoft 365 | Customer with Zoom and Microsoft 365, target for conversion to Teams | 
| Povolit vzdálenou práci – soutěžit (Lupa) bez Microsoft 365 | Zákazník s přiblížením, cíl pro převod na týmy | 
| Snížení nákladů a Správa – Microsoft 365 E3 cílené pro Microsoft 365 E5 | Stávající zákazník s Microsoft 365 E3, cíl pro Microsoft 365 E5 | 
| Snižte náklady a spravujte Microsoft 365 Business zákazníky v jazyce Basic a Business Standard, které cílí na Microsoft 365 Business Premium. | Stávající zákazníci Microsoft 365 Business Basic a Business Standard, cíl pro Microsoft 365 Business Premium | 
| Transformace produktivity organizace – PROPER Surface | Zákazník zobrazuje PROPER pro plochu. | 
| M365Cluster | Identifikuje PROPER zákazníka k nákupu Microsoft 365. Zaměřte se na cíl a vyhodnoťte clustery, protože budou poskytovat vyšší výnosy. Informujte se o nurture a informujte zákazníky jenom v případě, že je stále dostupná kapacita a vyhodnoťte zákazníky. | 
| M365Fit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro naše nejlepší malé nebo střední firmy (SMB) k porovnání zákazníků a zjištění, zda se jedná o potenciální schopnost pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
| M365Intent | Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení pro definování clusterů. Bodování záměru se aktualizuje měsíčně. | 
| SurfaceCluster | Identifikuje náchylnost zákazníka k nákupu Surface tím, že konsoliduje doporučení Fit and Intent (Přizpůsobit a záměr) do clusteru. Zaměřte se teď na a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání jenom v případě, že existuje kapacita po provedení funkce Act Now a Evaluate customers are targeted(Vyhodnotit zákazníky). | 
| SurfaceFit | Interní a externí datové body, které definují pevné údaje. Bodování fitů používá pro naše nejlepší databáze MB podobný model, který porovnává zákazníky a určuje, jestli jsou vhodné pro cloudové produkty Microsoftu. Vyhodnocování fitů se aktualizuje čtvrtletně. | 
| SurfaceIntent | Signály související se sociálních sítěmi a online chováním zákazníka definují záměr. Bodování záměru je přeocené na možnost Přizpůsobit, aby bylo možné definovat clustery. Bodování záměru se aktualizuje každý měsíc. | 
| O365Cluster | Identifikuje náchylnost zákazníka k nákupu Office 365. Zaměřte se hned a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání jenom v případě, že existuje kapacita, na které cílí zákazníci po provedení act now a evaluate. | 
| O365Fit | Interní a externí datové body, které definují pevné údaje. Bodování fitů používá k porovnání zákazníků podobný model pro naše nejlepší databáze, aby bylo možné porovnat zákazníky a zjistit, jestli se hodí pro cloudové produkty Microsoftu. Vyhodnocování fitů se aktualizuje čtvrtletně. | 
| O365Intent | Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení pro definování clusterů. Bodování záměru se aktualizuje měsíčně. | 
| M365UpsellCustomer | Určuje, jestli zákazník zobrazuje přeprodat PROPER pro Microsoft 365. | 
| Má Google | Určuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnictví produktů Google. | 
| Má AWS | Určuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnící produkty Amazon Web Services (AWS). | 
| Má EA | Určuje, jestli se jedná o prodloužení platnosti smlouvy Enterprise (EA) nebo předplatného EA. | 
| Má otevřené | Určuje, jestli je obnovování smlouva otevřené nebo otevřené hodnoty. | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloud stoupání – sestava PROPER v Dynamics 365**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ID MPN | ID Microsoft Partner Network | 
| Název partnera | Název partnera | 
| ID zákazníka | Číslo identifikátoru zákazníka | 
| Číslo DUNS | The Dun & Brad number of the customer who's scored for propensity | 
| Account Name | Název účtu | 
| Doména | Doména účtu | 
| Velikost organizace | Velikost organizace | 
| Obor | Odvětví, do které organizace patří | 
| Svisle | Svislá část zákazníka, u které se cítí skóre z úhludnosti, kterou identifikoval Microsoft, D&B a další oborové standardy
| Plošný | Geografická oblast umístění | 
| Pobočka | Pobočka zákazníka, u které se uje skóre z oblasti náchylnosti | 
| Sales Territory (Prodejní oblast) | Prodejní oblast zákazníka, u jehož skóre se skóruje náchylnost | 
| City (Město) | Zeměpisné umístění města | 
| Stav | Geografické umístění | 
| PSČ | PSČ organizace | 
| Země | Zeměpisné umístění země | 
| Segment | Segment trhu | 
| Dílčí segment | Dílčí podsegment trhu | 
| Souhrn typů SMC | Kategorizace zákazníka: Nejspravovanou uživatelskou základnou jsou zákazníci s více než 300 zaměstnanci, nejspravovanými výpočetními bázemi jsou zákazníci s tříletým potenciálem Azure 10 000 USD, střední firmy jsou zákazníci s více než 25 zaměstnanci a malé firmy jsou zákazníky s méně než 25 zaměstnanci. | 
| Nejspravované – výpočetní základ | Hlavní nespravované zákazníky – COMPUTE | 
| Hlavní nespravovaný – základ uživatele | Hlavní nespravované zákazníky – uživatelé | 
| IsNonProfit | Indikuje, jestli je organizace nezisková (Ano nebo ne). | 
| Aktivace digitálního prodeje-Microsoft 365-velikost sedadel >= 25 míst (model PROPER SalesPro) | Zákazník bez Dynamics 365. Velikost sedadla: 25 +. Partner by měl cílit na prodej Dynamics 365 SalesPro. | 
| Aktivace digitálního prodeje – Dynamics 365 SalesPro Proper (ACT nyní nebo Evaluate) | Zákazníci s vysokou mírou PROPER bez Dynamics 365. Partner by měl cílit na Dynamics 365 SalesPro. | 
| Správa finančních rizik & podvodů v místním prostředí – Dynamics – instalace pro základnu – Navision (model centrálních per pro firmy) | Stávající zákazník s místním Navision. Partner by měl cílit na Dynamics 365 Business Central. | 
| Správa finančních rizik & podvodů – místní instalace aplikace Dynamics AX – základní – Dynamics 365 (model PROPER Dynamics finance + operace) | Stávající zákazník s místní službou AX. Partner by měl cílit na operace Dynamics 365 finance +. | 
| Správa finančních rizik & podvodů v místním prostředí – místní instalace – velká místa (model centrálních per pro firmy) | Stávající zákazník s místními skvělými Plains. Partner by měl cílit na Dynamics 365 Business Central. | 
| Správa finančních rizik & podvody – Místní instalační základna Dynamics –Mon (model supenzity Business Central) | Stávající zákazník s místním předávkem Partner by měl cílit na Dynamics 365 Business Central. | 
| Správa finančních rizik & podvody – Místní instalační základna Dynamics – ostatní (model supenzí Business Central) | Stávající zákazník s jinými místními řešeními, která tu ještě nejsou uvedená Partner by měl cílit na Dynamics 365 Business Central. | 
| Sestavování agilní obchodních procesů – místní instalační základna Dynamics – AX/GP/SL/NAV/Other (model dynamics 365 propensity) | Sestavování agilní obchodních procesů – místní instalační základna Dynamics – AX/GP/SL/NAV/Other (model dynamics 365 propensity) | 
| Sestavování agilní obchodních procesů – dynamics compete base – Mendix/OutSystems/Salesforce (model dynamics 365 propensity) | Sestavování agilní obchodních procesů – Dynamics compete base – Mendix/OutSystems/Salesforce (model dynamics 365 propensity) | 
| Sestavování agilní obchodních procesů – instalační základna Dynamics 365 Finance + Operations | Stávající zákazníci Dynamics 365 Finance + Operations Partner pro Power Apps. | 
| Sestavování agilní obchodních procesů – instalační základna Dynamics 365 Business Central | Stávající zákazníci Dynamics 365 Business Central Partner pro Power Apps. | 
| Sestavování agilní obchodních procesů – instalační základna Dynamics 365 Customer Engagement | Stávající zákazníci Dynamics 365 Customer Engagement Partner pro Power Apps. | 
| Sestavte odolný dodavatelský řetězec – Windows a aktivujte první úlohu Dynamics 365 jako správu dodavatelských řetězců Dynamics 365 s zákazníky, kteří nepoužívají Oracle nebo SAP ERP (Enterprise Resource Planning). | Cílové zákazníky pro správu dodavatelských řetězců Dynamics 365 | 
| Sestavení odolného dodavatelského řetězce – meziprodejní Správa dodavatelských řetězců v Dynamics 365 a maloobchodu nebo obchodování s existujícími zákazníky Dynamics 365 Customer Engagement | Stávající zákazníci Dynamics 365 Customer Engagement cílí na spolupráci s prodejem dodavatelských dodavatelských řetězců v sadě Dynamics 365. | 
| Sestavení odolného dodavatelského řetězce – meziprodejní Správa dodavatelských řetězců v Dynamics 365 a maloobchod nebo prodej do Dynamics 365 Customer Engagement a Oracle nebo SAP | Stávající zákazníci Dynamics 365 Customer Engagement s Oracle nebo SAP pro cílení na správu dodavatelských řetězců Dynamics 365 | 
| D365BCCluster | Identifikuje PROPER zákazníka k nákupu Dynamics 365 Business Central. Zákazníci, kteří zobrazují PROPER pro firmu Business Central, budou mít střední a malou kategorii. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| D365BCFit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro náš nejlepší protokol SMB pro porovnání zákazníků a zjištění, jestli jsou potenciálními možnostmi pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
| D365BCIntent | Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení pro definování clusterů. Bodování záměru se aktualizuje měsíčně. | 
| D365FOCluster | Identifikuje náchylnost zákazníka k nákupu Dynamics 365 Finance and Operations. Zákazníci, kteří zobrazují sklony pro Finance + Operations, budou v horních nespravovaných kategoriích. Zaměřte se teď na a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání pouze v případě, že existuje kapacita po cílení na zákazníky, kteří se vyhodnocují, a vyhodnoťte je. | 
| D365FOFit | Interní a externí datové body, které definují pevné údaje. Bodování fitů používá pro náš nejlepší protokol SMB podobný model, který porovnává zákazníky a určuje, jestli jsou vhodné pro cloudové produkty Microsoftu. Vyhodnocování fitů se aktualizuje čtvrtletně. | 
| D365FOIntent | Signály související se sociálních sítěmi a online chováním zákazníka definují záměr. Bodování záměru je přeocené na možnost Přizpůsobit, aby bylo možné definovat clustery. Bodování záměru se aktualizuje každý měsíc. | 
| D365CECluster | Identifikuje náchylnost zákazníka k nákupu Dynamics 365 Customer Engagement. Zákazníci, kteří zobrazují sklony pro Customer Engagement, budou v kategoriích Střední a Malá. Zaměřte se teď na a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání jenom v případě, že existuje kapacita po cílení na zákazníky, kteří se vyhodnocují, a vyhodnoťte je. | 
| D365CEFit | Označuje Fit for Dynamics 365 Customer Engagement. | 
| D365CEIntent | Indikuje záměr pro zapojení zákaznických zákazníků Dynamics 365. | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Určuje, jestli má zákazník otevřené obnovení pro místní prostředí Dynamics AX nebo CRM. | 
| M365UpsellCustomer | Určuje, jestli zákazník zobrazuje přeprodat PROPER pro Microsoft 365. | 
| Má Google | Určuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnictví produktů Google. | 
| Má AWS | Určuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnící AWS produkty. | 
| Má EA | Určuje, jestli je obnovení předplatného EA nebo EA. | 
| Má otevřené | Určuje, jestli je obnovování smlouva otevřené nebo otevřené hodnoty. | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloudové prostoupání – sestava Azure Proper**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ID MPN | ID Microsoft Partner Network | 
| Název partnera | Název partnera | 
| ID zákazníka | Číslo identifikátoru zákazníka | 
| DUNS číslo | The Dun & Brad number of the customer who's scored for propensity | 
| Account Name | Název účtu | 
| Doména | Doména účtu | 
| Velikost organizace | Velikost organizace | 
| Obor | Obor | 
| Svisle | Svislá část zákazníka, u které se cítí skóre z úhludnosti, kterou identifikoval Microsoft, D&B a další oborové standardy | 
| Plošný | Geografická oblast umístění | 
| Pobočka | Pobočka zákazníka, u které se uje skóre z oblasti náchylnosti | 
| Sales Territory (Prodejní oblast) | Prodejní oblast zákazníka, u jehož skóre se skóruje náchylnost | 
| City (Město) | Zeměpisné umístění města | 
| Stav | Geografické umístění | 
| PSČ | PSČ organizace | 
| Země | Zeměpisné umístění země | 
| Segment | Segment trhu | 
| Dílčí segment | Dílčí podsegment trhu | 
| Souhrn typů SMC | Typ SMC | 
| Nejspravované – výpočetní základ | Nejspravovaná zákazníci – výpočetní prostředky | 
| Nejspravované – uživatelská základna | Hlavní nespravované zákazníky – uživatelé | 
| IsNonProfit | Indikuje, jestli je organizace nezisková (Ano nebo ne). | 
| Migrace – konce řádku Windows serveru – konce řádku Windows serveru IB s Promi v cloudu PROPER – 5 a licence | Zákazník, který má konce řádku místní Windows Server (tj. konce řádku verze nebo starší). Zákazník má 5 nebo více licencí. Zákazník, který má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – konce řádku Windows serveru – konce řádku Windows serveru IB s použitím PROPER v cloudu – <5 – licence | Zákazník, který má konce řádku místní Windows Server (tj. konce řádku verze nebo starší). Zákazník má méně než 5 licencí. Zákazník, který má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – konce řádku Windows serveru – konce řádku Windows serveru IB bez Proch PROPER v cloudu – 5 a licence | Zákazník, který má konce řádku místní Windows Server (tj. konce řádku verze nebo starší). Zákazník má více než 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – konce řádku Windows serveru – konce řádku Windows serveru IB bez Proch PROPER v cloudu – licence <5 | Zákazník, který má konce řádku místní Windows Server (tj. konce řádku verze nebo starší). Má méně než 5 licencí. Zákazník nemá skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – EOL SQL – EOL SQL Server IB s licencí Cloud Ascent – více než 5 licencí | Zákazník, který má místní EOL SQL Server (tj. verzi EOL nebo starší). Zákazník má více než 5 licencí. Zákazník má skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – EOL SQL – EOL SQL Server IB s licencí Cloud Ascent – <5 licencí | Zákazník, který má místní EOL SQL Server (tj. verzi EOL nebo starší). Má méně než 5 licencí. Zákazník, který má skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – EOL SQL – EOL SQL Server IB bez přechodu na cloud – více než 5 licencí | Zákazník, který má místní EOL SQL Server (tj. verzi EOL nebo starší). Zákazník má 5 nebo více licencí. Zákazník nemá skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – EOL SQL – EOL SQL Server IB bez přechodu ke cloudu – <5 licencí | Zákazník, který má místní EOL SQL Server (tj. verzi EOL nebo starší). Zákazník má méně než 5 licencí. Zákazník nemá skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – Migrace místního Windows Serveru – aktuální Windows Server IB s licencí Cloud Ascent – více než 5 licencí | Zákazník, který má aktuální místní Windows Server (tj. verzi novější než EOL). Zákazník má více než 5 licencí. Zákazník má skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – Migrace místního Windows Serveru – aktuální IB Windows Serveru s licencí Cloud Ascent – <5 licencí | Zákazník, který má aktuální místní Windows Server (tj. verzi novější než EOL). Zákazník má méně než 5 licencí. Zákazník má pro Azure skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – Migrace místního Windows Serveru – aktuální IB Windows Serveru bez přechodu ke cloudu – více než 5 licencí | Zákazník, který má aktuální místní Windows Server (tj. verzi novější než EOL). Zákazník má více než 5 licencí. Zákazník nemá skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – Migrace místního Windows Serveru – aktuální IB Windows Serveru bez licence Cloud Ascent – <5 licencí | Zákazník, který má aktuální místní Windows Server (tj. verzi novější než EOL). Zákazník má méně než 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace na virtuální počítače Azure SQL nebo SQL (VM) – aktuální SQL Server i s u cloudových PROPER – 5 a licence | Zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má 5 licencí. Zákazník má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace na virtuální počítače Azure SQL nebo SQL – aktuální SQL Server IB s použitím PROPER v cloudu – <5 | Zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má méně než 5 licencí. Zákazník má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace na virtuální počítače Azure SQL nebo SQL – aktuální SQL Server IB bez použití PROPER v cloudu – 5 a licence | Zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace na virtuální počítače Azure SQL nebo SQL – aktuální SQL Server IB bez použití PROPER v cloudu – <5 | Zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má méně než 5 licencí. Zákazník nemá skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – OSS – Migrace do open source databáze osspeare (OSS) | Stávající zákazník s libovolným z následujících produktů si konkuruje: PostgreSQL, MySQL, MariaDB. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – OSS – Linux v Azure | Stávající zákazník s Linuxem Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – SAP – SAP v Azure | Stávající zákazník se SASem Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – Windows Virtual Desktop – IB služby Vzdálená plocha | Identifikuje zákazníky s aktivní vzdálenou plochou Windows. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – Windows Virtual Desktop – Křížový prodej moderní práce do Azure/WVD | Identifikuje zákazníky s Microsoft 365 a nemá Azure. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – VMware IB | Stávající zákazník s tímto produktem: VMware. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – Citrix IB | Stávající zákazník s produktem: systémy Citrix. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Inovace – analýza-Power BI IB s vysokou mírou PROPER Azure | Zákazníci s předplatným a aktivním Power BI, včetně: Power BI-Standalone pro, Power BI – sady pro Azure, sady Power BI sady Office, Power BI sady – Microsoft 365 | 
| Enable-DevOps s GitHubem – Visual Studio/MSDN IB | Identifikuje zákazníky s aktivními verzemi sady Visual Studio. | 
| Windows Server Standard verze | Zobrazuje verzi nákupů Windows serveru Standard podle zákazníka. | 
| Windows Server Standard License | Zobrazí typ licence pro nákupy Windows serveru Standard podle zákazníka. | 
| Verze datového centra Windows serveru | Zobrazuje verzi Windows Data Center nákupů podle zákazníka. | 
| Licence datového centra Windows serveru | Zobrazí typ licence pro nákup datového centra Windows podle zákazníka. | 
| AzureFit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro náš nejlepší protokol SMB pro porovnání zákazníků a zjištění, jestli jsou potenciálními možnostmi pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
| AzureIntent | Signály související se sociálních sítěmi a online chováním zákazníka definují záměr. Bodování záměru je přeocené na možnost Přizpůsobit, aby bylo možné definovat clustery. Bodování záměru se aktualizuje každý měsíc. | 
| AzureCluster | Identifikuje náchylnost zákazníka k nákupu Azure tím, že konsoliduje doporučení Fit and Intent (Přizpůsobit a záměr) do clusteru. Zaměřte se teď na a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání pouze v případě, že existuje kapacita po cílení na zákazníky, kteří se vyhodnocují, a vyhodnoťte je. | 
| WindowsServerDataCenter_HasOpenRenewal | Určuje, jestli má zákazník otevřené prodloužení platnosti datacentra Windows Serveru. | 
| WindowsServerStandard_HasOpenRenewal | Určuje, jestli má zákazník otevřené prodloužení platnosti Windows Serveru Standard. | 
| AzureUpsellCustomer | Určuje, jestli se zákazníkovi zobrazuje sklon pro upsell pro Azure. | 
| Má Google | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící produkty Google. | 
| Má AWS | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící produkty AWS. | 
| Má EA | Určuje, jestli je prodloužení předplatného EA nebo EA. | 
| Má otevřené | Určuje, jestli je obnovování smlouva otevřené nebo otevřené hodnoty. | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Cloud stoupání – sestava PROPER obnovení smluv**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ID MPN | ID Microsoft Partner Network | 
| Název partnera | Název partnera | 
| ID zákazníka | Číslo identifikátoru zákazníka | 
| DUNS číslo | Telefonické připojení & Bradstreet číslo zákazníka, který je v hodnocení pro Proper | 
| Account Name | Název účtu | 
| Doména | Doména účtu | 
| Velikost organizace | Velikost organizace | 
| Obor | Obor | 
| Svisle | Svislá část zákazníka, u kterého se skóre v rámci PROPER identifikovali podle identifikace od Microsoftu, D&B a dalších oborových standardů | 
| Plošný | Zeměpisná oblast umístění | 
| Pobočka | Dceřiná společnost zákazníka, u kterého se má skóre na Proper | 
| Sales Territory (Prodejní oblast) | Prodejní teritorium zákazníka, u kterého se provádí hodnocení Proper | 
| City (Město) | Zeměpisná poloha města | 
| Stav | Zeměpisné umístění stavu | 
| PSČ | Poštovní směrovací číslo organizace | 
| Země | Zeměpisné umístění země | 
| Segment | Segment trhu | 
| Dílčí segment | Dílčí podsegment trhu | 
| Souhrn typů SMC | Typ SMC | 
| Nejspravované – výpočetní základ | Nejspravovaná zákazníci – výpočetní prostředky | 
| Nejspravované – uživatelská základna | Nejspravovaná zákazníci – uživatelé | 
| IsNonProfit | Určuje, jestli je organizace nezisková (Ano nebo Ne). | 
| Má Google | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící produkty AWS. | 
| Má AWS | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící produkty AWS. | 
| Azure Cluster | Identifikuje náchylnost zákazníka k nákupu Azure. Zaměřte se teď na a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání pouze v případě, že existuje kapacita po cílení na zákazníky, kteří se vyhodnocují, a vyhodnoťte je. | 
| D365 finance + provozní cluster | Identifikuje PROPER zákazníka k nákupu Dynamics 365 finance a operací. Zákazníci, kteří zobrazují PROPER pro finance a operace, budou v hlavních nespravovaných kategoriích. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| Cluster D365 CE | Identifikuje PROPER zákazníka k nákupu zákaznického zapojení Dynamics 365. Zákazníci, kteří zobrazují PROPER pro zapojení zákazníka, budou ve středních a malých kategoriích. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| Cluster D365 BC | Identifikuje PROPER zákazníka k nákupu Dynamics 365 Business Central. Zákazníci, kteří zobrazují PROPER pro firmu Business Central, budou mít střední a malou kategorii. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| Cluster Microsoft 365 | Identifikuje PROPER zákazníka k nákupu Microsoft 365. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| Licenční program | Určuje typ licenčního programu pro prodloužení platnosti. | 
| ID smlouvy | Identifikátor smlouvy | 
| Datum ukončení smlouvy | Koncové datum smlouvy | 
| Typ vypršení platnosti | Typ vypršení platnosti | 
| Vypršení tržeb | Výnosy spojené s vypršením platnosti předplatných | 
| Má EA | Určuje, jestli je prodloužení předplatného EA nebo EA. | 
| Má otevřený | Určuje, jestli je prodloužení smlouvou Open Nebo Open Value. | 
| Zákazník Azure Upsell | Určuje, jestli se zákazníkovi zobrazuje sklon pro upsell pro Azure. | 
| Microsoft 365 zákazníka upsell | Určuje, jestli zákazník u zákazníka zobrazuje kolísavost Microsoft 365 | 
| RevSumDivisionName | Určuje produkt, pro který je k dispozici prodloužení platnosti. | 

## <a name="next-steps"></a>Další kroky

Další informace najdete v tématu [Stažení sestav.](pci-download-reports.md)
