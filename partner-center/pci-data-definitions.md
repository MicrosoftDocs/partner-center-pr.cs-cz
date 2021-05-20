---
title: Definice dat Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dokument obsahuje seznam různých sestav a jejich definic dat, které si můžete stáhnout ze stránky Přehledy Stáhnout sestavu.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 721caed2d8b0e24940e7adedeb90cc689a82d2e7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152830"
---
# <a name="export--data-definitions"></a>Export – definice dat 

**Odpovídající role:** Prohlížeč sestav | Prohlížeč výkonných sestav

## <a name="introduction"></a>Úvod 

Pomocí centra Pro stahování sestav na řídicím panelu Přehledy můžete exportovat nezpracované datové sady. 

Různé sestavy, které si můžete stáhnout společně s jejich definicemi dat, jsou uvedené v následujících tabulkách: 

### <a name="partner-profile-report"></a>**Sestava profilu partnera**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ID MPN | Identifikátor Microsoft Partner Network (MPN) | 
| PartnerName | Název partnera | 
| PGA_MPNId | Identifikátor MPN globálního partnerského účtu | 
| PGA_PartnerName | Název globálního účtu partnera | 
| City (Město) | Město partnera | 
| Země | Země/ umístění partnera | 
| HierarchyLevel | Určuje, jestli se jedná o globální ID MPN nebo ID MPN umístění. | 

### <a name="customer-details-report"></a>**Sestava podrobností o zákazníkovi**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerName | Jméno zákazníka | 
| CustomerTenantId | Identifikátor tenanta zákazníka | 
| CustomerTpid | Identifikátor nejvyšší nadřazené položky zákazníka | 
| CustomerSegment | Segment zákazníka | 
| CustomerMarket | Zeměpisný trh zákazníka | 
| CustomerStatus | Stav zákazníka (aktivní nebo neaktivní) | 
| Produkt | Produkt prodal zákazník od MPN: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI nebo Microsoft Azure | 
| SKU | SKU produktu | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití a výnosy | 
| MPNId | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| PartnerLocation | Zeměpisné umístění partnera | 
| PartnerAttributionType | Typ přidělení partnera | 
| SalesChannel | Prodejní kanál | 
| AvailableSeats | Dostupné licencí | 
| Revenue (Výnosy) | Revenue in US dollars | 

### <a name="reseller-performance-report"></a>**Sestava výkonu prodejce**

> [!Note]
> Údaje o výnosech a ACR jsou k dispozici pouze uživatelům, kteří jsou diváky sestav vedení.

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ResellerMPNid | Identifikátor Microsoft Partner Network prodejce | 
| ResellerName | Jméno prodejce | 
| ResellerMarket | Země prodejce na trhu | 
| IndirectProviderMPNId | Identifikátor nepřímého poskytovatele Microsoft Partner Network | 
| IndirectProviderName | Název nepřímého poskytovatele | 
| Month (Měsíc) | Měsíc, pro který se hlásí využití a výnosy | 
| Produkt | Název produktu | 
| ID předplatného | Identifikátor předplatného | 
| AvailableSeats | Počet dostupných míst | 
| AssignedSeats | Počet přiřazených stanic | 
| BilledRevenueUSD | Fakturované výnosy v amerických dolarech | 
| CustomerName | Jméno zákazníka | 
| CustomerTPid | Identifikátor nejvyšší nadřazené položky zákazníka | 
| CustomerSegment | Segment zákazníka | 
| CustomerMarket | Zeměpisný trh zákazníka | 
| ResellerStatus | Stav prodejce | 

### <a name="subscription-details-report"></a>**Sestava Podrobnosti o předplatném**

>[!Note]
>Data o výnosech a ACR jsou k dispozici pouze uživatelům, kteří jsou správci sestav od manažera.

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| SubscriptionId | Identifikátor GUID předplatného | 
| SubscriptionStartDate | Počáteční datum odběru | 
| Datum ukončení předplatného | Koncové datum předplatného | 
| Stav předplatného | Stav předplatného (aktivní nebo churned) | 
| Month (Měsíc) | Měsíc, za který se hlásí využití a výnosy | 
| IsAutoRenew | Určuje, jestli je odběr autorenew (Ano nebo Ne). | 
| CustomerName | Jméno zákazníka | 
| CustomerTenantId | IDENTIFIKÁTOR GUID zákazníka | 
| CustomerTpid | Hlavní nadřazený identifikátor zákazníka | 
| CustomerSegment | Segment trhu zákazníka | 
| CustomerMarket | Geografický trh zákazníka | 
| Produkt | Produkt prodaný partnerem zákazníkovi | 
| SKU | SKU produktu | 
| ID MPN | Microsoft Partner Network ID partnera | 
| PartnerName | Název partnera | 
| PartnerLocation | Zeměpisné umístění partnera | 
| PartnerAttributionType | Typ přidělení pro předplatné | 
| SalesChannel | Kanál pro prodejce s přímým přístupem, CSP (Cloud Solution Provider) atd. | 
| AvailableSeats | Aktuální dostupné místo | 
| RevenueUSD | Tržby v amerických dolarech | 
| ID registrace | ID registrace předplatného | 

### <a name="azure-usage-report"></a>**Sestava využití Azure**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| SubscriptionId | Identifikátor GUID předplatného | 
| SubscriptionStartDate | Datum začátku předplatného | 
| SubscriptionEndDate | Datum konce předplatného | 
| Stav předplatného | Aktuální stav předplatného (Otevřené, Uzavřené, Aktivní nebo V období odkladu) | 
| Month (Měsíc) | Datum agregované podle měsíce | 
| ServiceName | Název služby Azure | 
| MeterCategory | Název kategorie měřiče | 
| Jednotky využití | Počet jednotek použitých během fakturačního cyklu | 
| CustomerName | Jméno zákazníka | 
| CustomerTenantId | ID tenanta zákazníka | 
| CustomerTpid | ID nejvyššího nadřazeného zákazníka | 
| CustomerSegment | Segment zákazníka | 
| CustomerMarket | Geografický trh zákazníka | 
| ID MPN | Microsoft Partner Network ID zákazníka | 
| PartnerName | Název partnera | 
| PartnerLocation | Zeměpisné umístění země partnera | 
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
| CustomerMarket | Zeměpisné umístění země na trhu zákazníka | 
| CustomerSegment | Segment zákazníka | 
| ID MPN | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| PartnerLocation | Zeměpisné umístění partnera | 
| PartnerAttributionType | Typ atribuce partnera | 

### <a name="enterprise-mobility-license-usage-report"></a>**Sestava využití licencí Enterprise Mobility**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenanta zákazníka | 
| CustomerTpid | ID nejvyššího nadřazeného zákazníka | 
| Název úlohy | Název úlohy Enterprise Mobility + Security (EMS) | 
| Month (Měsíc) | Měsíc, pro který se hlásí využití | 
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
| SubscriptionId | Identifikátor GUID předplatného | 
| SubscriptionStartDate | Počáteční datum odběru | 
| Datum ukončení předplatného | Koncové datum předplatného | 
| Stav předplatného | Stav předplatného | 
| Month (Měsíc) | Měsíc, pro který se hlásí využití | 
| RevSumDivisionName | Název dělení rev sum | 
| RevSumCategoryName | Název kategorie součetu revize | 
| SKU | SKU produktu | 
| SKUId | ID SKU produktu | 
| FreeVsPaidSKU | Určuje, jestli se jedná o bezplatnou nebo placenou SKU. | 
| SalesModel | Prodejní kanál, který se používá k prodeji předplatného | 
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
| ActiveSeats | Aktuální aktivní křesla | 
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
| ID SKU | ID SKU produktu | 
| FreeVsPaidSKU | Rozdíl bezplatné nebo placené SKU | 
| SalesModel (Model prodeje) | Prodejní model, který se používá k prodeji předplatného | 
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
| AvailableSeats | Aktuální dostupná místa | 
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
| Month (Měsíc) | Měsíc, pro který se hlásí využití | 
| 3P Název aplikace | Název aplikace Teams | 
| Počet uživatelů | Počet uživatelů pro aplikaci | 


### <a name="training-details-report"></a>**Sestava podrobností trénování**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ID aktivity trénování | Identifikátor trénování | 
| TrainingTitle (Trénování názvu) | Název školení | 
| Typ trénování | Typ školení (certifikace nebo zkouška) | 
| Jednotlivý_název_první_položky | Jméno zákazníka | 
| IndividualLastName | Příjmení zákazníka | 
| E-mail | ID osobního e-mailu zákazníka | 
| CorpEmail | ID e-mailu office zákazníka | 
| TrainingCompletionDate | Datum dokončení školení | 
| Month (Měsíc) | Měsíc, pro který se data oznamují | 
| IcMCP | Indikuje, jestli je uživatel Microsoft Certified Professional (MCP). | 
| MCPID | ID MCP uživatele | 
| MPNId | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| PartnerCityLocation | Zeměpisná poloha města partnera | 
| PartnerCountryLocation | Zeměpisná poloha země partnera | 

### <a name="microsoft-learn-report"></a>**Sestava Microsoft Learn**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| Uživatelské jméno | Jméno uživatele | 
| UserId | Identifikátor GUID uživatele | 
| Procvičení | Název školení | 
| Typ trénování | Typ školení (modul nebo studijní program) | 
| Produkty | Produkt, pro který je výukový modul použitelný | 
| Role | Příslušné role školení | 
| Datum dokončení | Datum dokončení trénování | 
| ID MPN | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| Země | Zeměpisné umístění země partnera | 

### <a name="competency-summary-and-history-report"></a>**Souhrn kompetencí a sestava historie**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| Název kompetence | Název kompetence | 
| CompetencyLevel | Úroveň kompetence (zlaté nebo zlaté) | 
| Stav kompetence | Aktuální stav kompetence (Aktivní, Neaktivní nebo V období odkladu) | 
| Datum zahájení kompetencí | Počáteční datum kompetence | 
| CompetencyEndDate | Koncové datum kompetence | 

### <a name="competency-performance-report"></a>**Sestava o výkonu kompetence**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CompetencyName | Název kompetence | 
| CompetencyAttainmentOptionName | Název možnosti dosažení kompetence | 
| Month (Měsíc) | Měsíc, pro který jsou hlášeny metriky | 
| MetricName | Název metriky, která souvisí s kompetencí | 
| MetricMonthlyContribution | Měsíční příspěvek metriky | 
| TTMAggregate | Agregovaná metrika pro koncové 12 měsíců | 
| AnniversaryYearAggregate | Agregovaná metrika pro aktuální rok výročí | 
| GoldThreshold | Požadavek na výkon pro splnění zlaté kompetence | 
| SilverThreshold | Požadavek na výkon pro uspokojení stříbrné kompetence | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Ascent cloudu – Microsoft 365 o nárocích**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ID MPN | Microsoft Partner Network ID | 
| Název partnera | Název partnera | 
| ID zákazníka | Číslo identifikátoru zákazníka | 
| Číslo DUNS | The Dun & Brad neschůdný (D&B) zákazníka, který má skóre z řad náchylnosti. | 
| Account Name | Název účtu | 
| Doména | Doména účtu | 
| Velikost organizace | Velikost organizace | 
| Obor | Odvětví, do které organizace patří | 
| Svisle | Svislá část zákazníka, u které se určená sklony identifikovala společnost Microsoft, společnost D&B a další oborové standardy. | 
| Plošný | Geografická oblast umístění | 
| Pobočka | Pobočka zákazníka, u které se uje skóre z oblasti náchylnosti | 
| Sales Territory (Prodejní oblast) | Prodejní oblast zákazníka, u jehož skóre se skóruje sklon | 
| City (Město) | Zeměpisné umístění města organizace | 
| Stav | Zeměpisné umístění organizace | 
| PSČ | PSČ organizace | 
| Země | Zeměpisné umístění země organizace | 
| Segment | Segment trhu | 
| Dílčí segment | Segmentace trhu | 
| Shrnutí typu SMC | Typ SMC | 
| Hlavní nespravovaný – základ COMPUTE | Hlavní nespravované zákazníky – COMPUTE | 
| Hlavní nespravovaný – základ uživatele | Hlavní nespravované zákazníky – uživatel | 
| IsNonProfit | Indikuje, jestli je organizace nezisková (Ano nebo ne). | 
| Povolit vzdálený pracovní cíl Exchange Online | Zákazníci, kteří mají aktivní předplatné Exchange Online, přeprodat Microsoft 365 | 
| Povolit vzdálenou práci – místní akvizici (aktuální verze) s licencemi pro PROPER v cloudu – + 10 | Zákazníka, který má stávajícího místního Office nebo klienta Windows. To znamená, že verze klienta je novější než verze konce životnosti (konce řádku). Zákazník má 10 nebo více licencí. Zákazník, který má skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní akvizici (aktuální verze) s licencemi pro PROPER v cloudu – <10 | Zákazník, který má aktuálního místního klienta Office nebo Windows (tj. verzi novější než EOL). Zákazník má méně než 10 licencí. Zákazník, který má skóre sklonu. Partner by měl cílit na převod na Microsoft 365. | 
| Povolení vzdálené práce – místní pořízení (aktuální verze) bez licence Cloud Ascent – +10 licencí | Zákazník, který má aktuálního místního klienta Office nebo Windows (tj. verzi novější než EOL). Zákazník má 10 nebo více licencí. Zákazník nemá skóre sklonu. Partner by měl cílit na převod na Microsoft 365. | 
| Povolení vzdálené práce – místní získání (aktuální verze) bez licence Cloud Ascent – <10 licencí | Zákazník, který má aktuálního místního klienta Office nebo Windows (tj. verzi novější než EOL). Zákazník má méně než 10 licencí. Zákazník nemá skóre sklonu. Partner by měl cílit na převod na Microsoft 365. | 
| Povolení vzdálené práce – místní získání (verze EOL) s licencí Cloud Ascent – +10 licencí | Zákazník, který má místního klienta Office nebo Windows EOL (tj. verzi EOL nebo starší). Zákazník má 10 nebo více licencí. Zákazník má skóre sklonu. Partner by měl cílit na převod na Microsoft 365. | 
| Povolení vzdálené práce – místní získání (verze EOL) s licencí Cloud Ascent – <10 licencí | Zákazník, který má konce řádku místního Office nebo klienta Windows (to znamená, že konce řádku verze nebo starší). Zákazník má méně než 10 licencí. Zákazník má skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní pořízení (verze konce řádku) bez cloudových PROPER – + 10 licencí | Zákazník, který má stávajícího místního Office nebo klienta Windows (tj. verze konce řádku nebo starší). Zákazník má 10 nebo více licencí. Zákazník nemá skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní pořízení (konce řádku verze) bez cloudových PROPER – <10 | Zákazník, který má stávajícího místního Office nebo klienta Windows (tj. verze konce řádku nebo starší). Zákazník má méně než 10 licencí. Zákazník nemá skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálený pracovní postup s vysokou mírou prohlídky pro Microsoft 365 (ACT NowithEvaluate) | Zákazník v potenciálním zákazníkovi s vysokou mírou PROPER pro Microsoft 365 | 
| Povolení vzdálené práce – soutěžování (přiblížení) s Microsoft 365 | Zákazník s přiblížením a Microsoft 365 cíli pro převod na týmy | 
| Povolit vzdálenou práci – soutěžit (Lupa) bez Microsoft 365 | Zákazník s přiblížením, cíl pro převod na týmy | 
| Snížení nákladů a správy – Microsoft 365 E3 pro Microsoft 365 E5 | Stávající zákazník s Microsoft 365 E3, cíl pro Microsoft 365 E5 | 
| Snížení nákladů a správy – zákazníci Microsoft 365 Business Basic a Business Standard cílí na Microsoft 365 Business Premium | Stávající Microsoft 365 Business Basic a Business Standard, cíl pro Microsoft 365 Business Premium | 
| Transformace produktivity organizace – náchylnost k Surface | Zákazník zobrazuje sklon pro Surface | 
| M365Cluster | Identifikuje náchylnost zákazníka k nákupu Microsoft 365. Zaměřte se hned a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání jenom v případě, že existuje kapacita, na které cílí zákazníci po provedení act now a evaluate. | 
| M365Fit | Interní a externí datové body, které definují pevné údaje. Bodování fitů používá pro naše nejlepší malé nebo střední firmy (SME) podobný model, pomocí něj můžete porovnat zákazníky a zjistit, jestli jsou vhodné pro cloudové produkty Microsoftu. Vyhodnocování fitů se aktualizuje čtvrtletně. | 
| M365Intent | Signály související se sociálních sítěmi a online chováním zákazníka definují záměr. Bodování záměru je přeocené na možnost Přizpůsobit, aby bylo možné definovat clustery. Bodování záměru se aktualizuje každý měsíc. | 
| SurfaceCluster | Identifikuje náchylnost zákazníka k nákupu Surface tím, že konsoliduje doporučení Fit and Intent (Přizpůsobit a záměr) do clusteru. Zaměřte se na cíl a vyhodnoťte clustery, protože budou poskytovat vyšší výnosy. Informujte se o nurture a informujte zákazníky jenom v případě, že je stále dostupná kapacita a vyhodnoťte zákazníky. | 
| SurfaceFit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro naše nejlepší SMB k porovnání zákazníků a zjištění, jestli jsou potenciálními produkty pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
| SurfaceIntent | Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení pro definování clusterů. Bodování záměru se aktualizuje měsíčně. | 
| O365Cluster | Identifikuje PROPER zákazníka k nákupu Office 365. Zaměřte se na cíl a vyhodnoťte clustery, protože budou poskytovat vyšší výnosy. Informujte se o nurture a informujte zákazníky jenom v případě, že je stále dostupná kapacita a vyhodnoťte zákazníky. | 
| O365Fit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro naše nejlepší SMB k porovnání zákazníků a zjištění, jestli jsou potenciálními produkty pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
| O365Intent | Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je přeocené na možnost Přizpůsobit, aby bylo možné definovat clustery. Bodování záměru se aktualizuje každý měsíc. | 
| M365UpsellCustomer | Určuje, jestli zákazník u zákazníka zobrazuje kolísavost Microsoft 365 | 
| Má Google | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící produkty Google. | 
| Má AWS | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící Amazon Web Services (AWS). | 
| Má EA | Určuje, jestli je prodloužení smlouvou Enterprise (EA) nebo předplatným EA. | 
| Má otevřený | Určuje, jestli je prodloužení smlouvou Open Nebo Open Value. | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Ascent cloudu – sestava sklonů Dynamics 365**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ID MPN | Microsoft Partner Network ID | 
| Název partnera | Název partnera | 
| ID zákazníka | Číslo identifikátoru zákazníka | 
| Číslo DUNS | The Dun & Brad number of the customer who's scored for propensity | 
| Account Name | Název účtu | 
| Doména | Doména účtu | 
| Velikost organizace | Velikost organizace | 
| Obor | Odvětví, do kterého organizace patří | 
| Svisle | Svislá část zákazníka, u kterého se skóre v rámci PROPER identifikovali podle identifikace od Microsoftu, D&B a dalších oborových standardů
| Plošný | Zeměpisná oblast umístění | 
| Pobočka | Dceřiná společnost zákazníka, u kterého se má skóre na Proper | 
| Sales Territory (Prodejní oblast) | Prodejní teritorium zákazníka, u kterého se provádí hodnocení Proper | 
| City (Město) | Zeměpisná poloha města | 
| Stav | Zeměpisné umístění stavu | 
| PSČ | Poštovní směrovací číslo organizace | 
| Země | Zeměpisná poloha země | 
| Segment | Segment trhu | 
| Dílčí segment | Segmentace trhu | 
| Shrnutí typu SMC | Kategorizace zákazníka: hlavní nespravované uživatelské základy jsou zákazníky, kteří mají více než 300 zaměstnanců, hlavní nespravované výpočetní základy jsou zákazníci s USD10em, 3000 v rámci Azure tři roky jsou zákazníky s 25 zaměstnanci nebo vyšší a malým firmám jsou zákazníci s méně než 25 zaměstnanci. | 
| Hlavní nespravovaný – základ COMPUTE | Hlavní nespravované zákazníky – COMPUTE | 
| Hlavní nespravovaný – základ uživatele | Nejspravovaná zákazníci – uživatelé | 
| IsNonProfit | Určuje, jestli je organizace nezisková (Ano nebo Ne). | 
| Aktivace digitálního prodeje – Microsoft 365 – velikost >= 25 licencí (model s licencí SalesPro) | Zákazník bez Dynamics 365. Velikost místa: 25+. Partner by měl cílit na křížový prodej Dynamics 365 SalesPro. | 
| Aktivace digitálního prodeje – Dynamics 365 SalesPropensity (jednat hned nebo vyhodnotit) | Zákazníci s vysokou náchylností bez Dynamics 365. Partner by měl cílit na Dynamics 365 SalesPro. | 
| Řízení finančních rizik & podvodu – Místní instalační základna Dynamics – Navision (model náchylnosti k Business Central) | Stávající zákazník s místním Navision. Partner by měl cílit na Dynamics 365 Business Central. | 
| Správa finančních rizik & podvodu – Místní instalační základna Dynamics – Dynamics AX (dynamics 365 Finance + Operations Propensity model) | Stávající zákazník s místní osou AX Partner by měl cílit na Dynamics 365 Finance + Operations. | 
| Řízení finančních rizik & podvodu – Místní instalační základna Dynamics – Great Plains (model náchylnosti k Business Central) | Stávající zákazník s místními pláněmi Great Plains Partner by měl cílit na Dynamics 365 Business Central. | 
| Řízení finančních rizik & podvodu – Místní instalační základna Dynamics –Mon (model náchylnosti k Business Central) | Stávající zákazník s místní Šalamounovy ostrovy Partner by měl cílit na Dynamics 365 Business Central. | 
| Správa finančních rizik & podvodů v místním prostředí – místní instalace (model centrálních per pro firmy) | Stávající zákazník s dalšími místními řešeními, která ještě nejsou v seznamu uvedená. Partner by měl cílit na Dynamics 365 Business Central. | 
| Sestavování agilních podnikových procesů – Dynamics – místní instalace – základní – AX/GP/SL/NAV/ostatní (model PROPER Dynamics 365) | Sestavování agilních podnikových procesů – Dynamics – místní instalace – základní – AX/GP/SL/NAV/ostatní (model PROPER Dynamics 365) | 
| Vytváření agilních obchodních procesů – Dynamics konkurenční báze – Mendix/subsystéms/Salesforce (model PROPER Dynamics 365) | Vytváření agilních obchodních procesů – Dynamics konkurenční báze – Mendix/subsystéms/Salesforce (model PROPER Dynamics 365) | 
| Vytváření agilních obchodních procesů – základ pro Dynamics 365 finance + Operations Install | Stávající zákazníci s Dynamics 365 financemi a provozními operacemi. Partner pro cílení Power Apps. | 
| Sestavování agilních obchodních procesů – základ instalace Dynamics 365 Business Central | Stávající zákazníci s obchodním ústředním odvětvím Dynamics 365. Partner pro cílení Power Apps. | 
| Vytváření agilních obchodních procesů – základ pro instalaci Dynamics 365 Customer Engagement | Stávající zákazníci Dynamics 365 Customer Engagement. Partner pro cílení Power Apps. | 
| Sestavte odolný dodavatelský řetězec – Windows a aktivujte první úlohu Dynamics 365 jako správu dodavatelských řetězců Dynamics 365 s zákazníky, kteří nepoužívají Oracle nebo SAP ERP (Enterprise Resource Planning). | Cílové zákazníky pro správu dodavatelských řetězců Dynamics 365 | 
| Vytvoření odolného dodavatelského řetězce – křížové prodáte Dynamics 365 Supply Chain Management a/nebo Retail or Commerce stávajícím zákazníkům Dynamics 365 Customer Engagement | Stávající zákazníci Dynamics 365 Customer Engagement, kteří se mají zaměřit na řízení dodavatelského řetězce Dynamics 365 napříč prodeji. | 
| Vytvoření odolného dodavatelského řetězce – křížové prodeje pro Dynamics 365 Supply Chain Management a/nebo Retail or Commerce do Dynamics 365 Customer Engagement a Oracle nebo SAP | Stávající zákazníci Dynamics 365 Customer Engagement s Oraclem nebo SAP pro správu dodavatelského řetězce Dynamics 365 | 
| D365BCCluster | Identifikuje náchylnost zákazníka k nákupu Dynamics 365 Business Central. Zákazníci, kteří zobrazují sklon pro Business Central, budou v kategoriích Střední a Malá. Zaměřte se teď a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání pouze v případě, že existuje kapacita po cílení na zákazníky, kteří se vyhodnocují, a vyhodnoťte je. | 
| D365BCFit | Interní a externí datové body, které definují pevné údaje. Bodování fitů používá pro náš nejlepší protokol SMB podobný model, který porovnává zákazníky a určuje, jestli jsou vhodné pro cloudové produkty Microsoftu. Vyhodnocování fitů se aktualizuje čtvrtletně. | 
| D365BCIntent | Signály související se sociálních sítěmi a online chováním zákazníka definují záměr. Bodování záměru je přeocené na možnost Přizpůsobit, aby bylo možné definovat clustery. Bodování záměru se aktualizuje každý měsíc. | 
| D365FOCluster | Identifikuje náchylnost zákazníka k nákupu Dynamics 365 Finance and Operations. Zákazníci, kteří zobrazují sklony pro Finance + Operations, budou v horních nespravovaných kategoriích. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| D365FOFit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro náš nejlepší protokol SMB pro porovnání zákazníků a zjištění, jestli jsou potenciálními možnostmi pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
| D365FOIntent | Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení pro definování clusterů. Bodování záměru se aktualizuje měsíčně. | 
| D365CECluster | Identifikuje PROPER zákazníka k nákupu zákaznického zapojení Dynamics 365. Zákazníci, kteří zobrazují PROPER pro zapojení zákazníka, budou ve středních a malých kategoriích. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| D365CEFit | Indikuje přizpůsobení pro zákaznickou zapojení Dynamics 365. | 
| D365CEIntent | Indikuje záměr pro zapojení zákaznických zákazníků Dynamics 365. | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Určuje, jestli má zákazník otevřené prodloužení pro místní DYNAMICS AX nebo CRM. | 
| M365UpsellCustomer | Určuje, jestli zákazník u zákazníka zobrazuje kolísavost Microsoft 365 | 
| Má Google | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící produkty Google. | 
| Má AWS | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící produkty AWS. | 
| Má EA | Určuje, jestli je prodloužení předplatného EA nebo EA. | 
| Má otevřený | Určuje, jestli je prodloužení smlouvou Open Nebo Open Value. | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud Ascent – sestava náchylnosti k Azure**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ID MPN | Microsoft Partner Network ID | 
| Název partnera | Název partnera | 
| ID zákazníka | Číslo identifikátoru zákazníka | 
| Číslo DUNS | The Dun & Brad number of the customer who's scored for propensity | 
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
| Země | Zeměpisná poloha země | 
| Segment | Segment trhu | 
| Dílčí segment | Segmentace trhu | 
| Shrnutí typu SMC | Typ SMC | 
| Hlavní nespravovaný – základ COMPUTE | Hlavní nespravované zákazníky – COMPUTE | 
| Hlavní nespravovaný – základ uživatele | Hlavní nespravované zákazníky – uživatelé | 
| IsNonProfit | Určuje, jestli je organizace nezisková (Ano nebo Ne). | 
| Migrace – EOL Windows Server – EOL Windows Server IB s licencí Cloud Ascent – více než 5 licencí | Zákazník, který má EOL místní Windows Server (tj. verzi EOL nebo starší). Zákazník má 5 nebo více licencí. Zákazník, který má skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – EOL Windows Server – EOL Windows Server IB s licencí Cloud Ascent – <5 licencí | Zákazník, který má EOL místní Windows Server (tj. verzi EOL nebo starší). Zákazník má méně než 5 licencí. Zákazník, který má skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – EOL Windows Server – EOL Windows Server IB bez přechodu na cloud – více než 5 licencí | Zákazník, který má EOL místní Windows Server (tj. verzi EOL nebo starší). Zákazník má více než 5 licencí. Zákazník nemá skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – EOL Windows Server – EOL Windows Server IB bez přechodu na cloud – <5 licencí | Zákazník, který má EOL místní Windows Server (tj. verzi EOL nebo starší). Má méně než 5 licencí. Zákazník nemá skóre sklonu. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – konce řádku SQL-konce řádku SQL Server IB s Promi cloudových PROPER – 5 a licence | Zákazník, který má konce řádku místní SQL Server (tj. konce řádku verze nebo starší). Zákazník má 5 licencí. Zákazník má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – konce řádku SQL-konce řádku SQL Server IB a u cloudových PROPER – <5 licencí | Zákazník, který má konce řádku místní SQL Server (tj. konce řádku verze nebo starší). Má méně než 5 licencí. Zákazník, který má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – konce řádku SQL-konce řádku SQL Server IB bez použití PROPER v cloudu – 5 a licence | Zákazník, který má konce řádku místní SQL Server (tj. konce řádku verze nebo starší). Zákazník má 5 nebo více licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – konce řádku SQL-konce řádku SQL Server IB bez použití PROPER v cloudu – <5 licencí | Zákazník, který má konce řádku místní SQL Server (tj. konce řádku verze nebo starší). Zákazník má méně než 5 licencí. Zákazník nemá skóre proper. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – Migrace místního Windows Serveru – aktuální IB Windows Serveru s licencí Cloud Ascent – více než 5 licencí | Zákazník, který má aktuální místní Windows Server (tj. verzi novější než EOL). Zákazník má více než 5 licencí. Zákazník má skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – Migrace místního Windows Serveru – aktuální IB Windows Serveru s licencí Cloud Ascent – <5 licencí | Zákazník, který má aktuální místní Windows Server (tj. verzi novější než EOL). Zákazník má méně než 5 licencí. Zákazník má pro Azure skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – Migrace místního Windows Serveru – aktuální IB Windows Serveru bez licence Cloud Ascent – více než 5 licencí | Zákazník, který má aktuální místní Windows Server (tj. verzi novější než EOL). Zákazník má více než 5 licencí. Zákazník nemá skóre sklonu. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – Migrace místního Windows Serveru – aktuální IB Windows Serveru bez licence Cloud Ascent – <5 licencí | Zákazník, který má aktuální místní Windows Server (tj. verzi novější než EOL). Zákazník má méně než 5 licencí. Zákazník nemá skóre sklonu. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace na virtuální počítače Azure SQL nebo SQL (VM) – aktuální SQL Server i s u cloudových PROPER – 5 a licence | Zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má 5 licencí. Zákazník má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace na virtuální počítače Azure SQL nebo SQL – aktuální SQL Server IB s použitím PROPER v cloudu – <5 | Zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má méně než 5 licencí. Zákazník má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace na virtuální počítače Azure SQL nebo SQL – aktuální SQL Server IB bez použití PROPER v cloudu – 5 a licence | Zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace na virtuální počítače Azure SQL nebo SQL – aktuální SQL Server IB bez použití PROPER v cloudu – <5 | Zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má méně než 5 licencí. Zákazník nemá skóre proper. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – OSS – Migrace do open source databáze osspeare (OSS) | Stávající zákazník s libovolným z následujících produktů si konkuruje: PostgreSQL, MySQL, MariaDB. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – OSS – Linux v Azure | Stávající zákazník s Linuxem Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – SAP – SAP v Azure | Stávající zákazník se SAP. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – Windows Virtual Desktop – IB služby Vzdálená plocha | Identifikuje zákazníky s aktivní vzdálenou plochou Windows. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – Windows Virtual Desktop – Křížové prodej moderní práce do Azure/WVD | Identifikuje zákazníky s Microsoft 365 a nemá Azure. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – VMware IB | Stávající zákazník s tímto produktem: VMware. Partner by měl tohoto zákazníka cílit na migraci do Azure. | 
| Migrace – Citrix IB | Stávající zákazník s produktem: systémy Citrix. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Inovace – analýza-Power BI IB s vysokou mírou PROPER Azure | Zákazníci s předplatným a aktivním Power BI, včetně: Power BI-Standalone pro, Power BI – sady pro Azure, sady Power BI sady Office, Power BI sady – Microsoft 365 | 
| Enable-DevOps s GitHubem – Visual Studio/MSDN IB | Identifikuje zákazníky s aktivními verzemi sady Visual Studio. | 
| Windows Server Standard verze | Zobrazuje verzi nákupů Windows serveru Standard podle zákazníka. | 
| Windows Server Standard License | Zobrazí typ licence pro nákupy Windows serveru Standard podle zákazníka. | 
| Verze datového centra Windows serveru | Zobrazuje verzi Windows Data Center nákupů podle zákazníka. | 
| Licence datového centra Windows serveru | Zobrazí typ licence pro nákup datového centra Windows podle zákazníka. | 
| AzureFit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro náš nejlepší protokol SMB pro porovnání zákazníků a zjištění, jestli jsou potenciálními možnostmi pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
| AzureIntent | Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je přeocené na možnost Přizpůsobit, aby bylo možné definovat clustery. Bodování záměru se aktualizuje každý měsíc. | 
| AzureCluster | Identifikuje náchylnost zákazníka k nákupu Azure tím, že konsoliduje doporučení Fit and Intent (Přizpůsobit a záměr) do clusteru. Zaměřte se teď a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání pouze v případě, že existuje kapacita po cílení na zákazníky, kteří se vyhodnocují, a vyhodnoťte je. | 
| WindowsServerDataCenter_HasOpenRenewal | Určuje, jestli má zákazník otevřené prodloužení platnosti datacentra Windows Serveru. | 
| WindowsServerStandard_HasOpenRenewal | Určuje, jestli má zákazník otevřené prodloužení platnosti pro Windows Server Standard. | 
| AzureUpsellCustomer | Určuje, jestli zákazník zobrazuje kolísavost upsell pro Azure. | 
| Má Google | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící produkty Google. | 
| Má AWS | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící produkty AWS. | 
| Má EA | Určuje, jestli je prodloužení předplatného EA nebo EA. | 
| Má otevřený | Určuje, jestli je prodloužení smlouvou Open Nebo Open Value. | 

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
| Země | Zeměpisná poloha země | 
| Segment | Segment trhu | 
| Dílčí segment | Dílčí podsegment trhu | 
| Souhrn typů SMC | Typ SMC | 
| Nejspravované – výpočetní základ | Nejspravované zákazníky – výpočetní prostředky | 
| Nejspravované – uživatelská základna | Nejspravovaná zákazníci – uživatelé | 
| IsNonProfit | Určuje, jestli je organizace nezisková (Ano nebo Ne). | 
| Má Google | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící produkty AWS. | 
| Má AWS | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící produkty AWS. | 
| Azure Cluster | Identifikuje náchylnost zákazníka k nákupu Azure. Zaměřte se teď a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání pouze v případě, že existuje kapacita po cílení na zákazníky, kteří se vyhodnocují, a vyhodnoťte je. | 
| D365 Finance + Operations Cluster | Identifikuje náchylnost zákazníka k nákupu Dynamics 365 Finance and Operations. Zákazníci, kteří zobrazují PROPER pro finance a operace, budou v hlavních nespravovaných kategoriích. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| Cluster D365 CE | Identifikuje PROPER zákazníka k nákupu zákaznického zapojení Dynamics 365. Zákazníci, kteří zobrazují PROPER pro zapojení zákazníka, budou ve středních a malých kategoriích. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| Cluster D365 BC | Identifikuje PROPER zákazníka k nákupu Dynamics 365 Business Central. Zákazníci, kteří zobrazují PROPER pro firmu Business Central, budou mít střední a malou kategorii. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| Cluster Microsoft 365 | Identifikuje PROPER zákazníka k nákupu Microsoft 365. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| Licenční program | Identifikuje typ licenčního programu pro obnovení. | 
| ID smlouvy | Identifikátor smlouvy | 
| Datum ukončení smlouvy | Koncové datum smlouvy | 
| Typ vypršení platnosti | Typ vypršení platnosti | 
| Vypršení tržeb | Výnosy spojené s vypršením platnosti předplatných | 
| Má EA | Určuje, jestli je prodloužení předplatného EA nebo EA. | 
| Má otevřený | Určuje, jestli je prodloužení smlouvou Open Nebo Open Value. | 
| Zákazník Azure Upsell | Určuje, jestli zákazník zobrazuje kolísavost upsell pro Azure. | 
| Microsoft 365 zákazníka upsell | Určuje, jestli zákazník u zákazníka zobrazuje kolísavost Microsoft 365 | 
| RevSumDivisionName | Určuje produkt, pro který je k dispozici prodloužení platnosti. | 

## <a name="next-steps"></a>Další kroky

Další informace najdete v tématu [Stažení sestav.](pci-download-reports.md)
