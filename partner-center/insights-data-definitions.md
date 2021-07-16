---
title: Definice dat Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: dokument obsahuje seznam různých sestav a jejich definicí dat, které můžete stáhnout ze stránky sestavy stáhnout Přehledy.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c77f5eb97771c4768f76b8d35c0d4493c5070ff2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376474"
---
# <a name="export--data-definitions"></a>Export – definice dat 

**Příslušné role**: Prohlížeč sestav | Prohlížeč sestav Executive

## <a name="introduction"></a>Úvod 

pomocí centra pro stažení sestav na řídicím panelu Přehledy můžete exportovat nezpracované datové sady. 

Různé sestavy, které si můžete stáhnout spolu s definicemi jejich dat, jsou uvedené v následujících tabulkách: 

### <a name="partner-profile-report"></a>**Sestava profil partnera**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| MPNId | ID Microsoft Partner Network (MPN)| 
| PartnerName | Název partnera | 
| PGA_MPNId | Identifikátor účtu MPN globálního účtu partnera | 
| PGA_PartnerName | Název globálního účtu partnera | 
| City (Město) | Město, kde se nachází partner | 
| Země | Umístění země partnera | 
| HierarchyLevel | Označuje, jestli se jedná o globální ID MPN, nebo ID MPN umístění. | 

### <a name="customer-details-report"></a>**Sestava Podrobnosti o zákazníkovi**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerName | Jméno zákazníka | 
| CustomerTenantId | Identifikátor tenanta zákazníka | 
| CustomerTpid | Identifikátor nejvyšší nadřazené položky zákazníka | 
| CustomerSegment | Segment zákazníka | 
| CustomerMarket | Zeměpisný trh zákazníka | 
| CustomerStatus | Stav zákazníka (aktivní nebo neaktivní) | 
| Produkt | produkt prodávaný zákazníkem MPN: Office 365, Dynamics 365, Enterprise mobility a zabezpečení, Power BI nebo Microsoft Azure | 
| SKU | SKU produktu | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití a výnosy | 
| MPNId | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| PartnerLocation | Zeměpisné umístění partnera | 
| PartnerAttributionType | Typ přidělení partnera | 
| SalesChannel | Prodejní kanál | 
| AvailableSeats | Dostupná místa | 
| RevenueUSD | Tržby v amerických dolarech | 

### <a name="reseller-performance-report"></a>**Sestava o výkonu prodejce**

> [!Note]
> Data o výnosech a tržbách za Azure (ACR) jsou k dispozici pouze uživatelům, kteří jsou správci sestav od vedoucího.

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ResellerMPNid | Identifikátor Microsoft Partner Network prodejce | 
| ResellerName | Jméno prodejce | 
| ResellerMarket | Prodejce země na trhu | 
| IndirectProviderMPNId | Identifikátor Microsoft Partner Network nepřímého zprostředkovatele | 
| IndirectProviderName | Název nepřímého zprostředkovatele | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití a výnosy | 
| Produkt | Název produktu | 
| SubscriptionID | Identifikátor předplatného | 
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
| SubscriptionId | GUID předplatného | 
| Datum_zahájení_předplatného | Počáteční datum odběru | 
| Datum ukončení předplatného | Koncové datum předplatného | 
| Stav předplatného | Stav předplatného (aktivní nebo churned) | 
| Month (Měsíc) | Měsíc, pro který se vykazují údaje o využití a výnosech | 
| IsAutoRenew | Určuje, jestli je odběr autorenewed (Ano nebo Ne). | 
| CustomerName | Jméno zákazníka | 
| CustomerTenantId | IDENTIFIKÁTOR GUID zákazníka | 
| CustomerTpid | Nadřazený identifikátor zákazníka | 
| CustomerSegment | Segment trhu zákazníka | 
| CustomerMarket | Geografický trh zákazníka | 
| Produkt | Produkt prodaný partnerem zákazníkovi | 
| SKU | SKU produktu | 
| ID MPN | Microsoft Partner Network ID partnera | 
| PartnerName | Název partnera | 
| PartnerLocation | Zeměpisné umístění partnera | 
| PartnerAttributionType | Typ atribuce pro předplatné | 
| SalesChannel | Kanál prodeje – Přímý, Cloud Solution Provider (CSP) a tak dále | 
| AvailableSeats | Aktuální dostupná místa | 
| Revenue (Výnosy) | Revenue in US dollars | 
| ID registrace | ID registrace předplatného | 

### <a name="azure-usage-report"></a>**Sestava využití Azure**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| SubscriptionId | GUID předplatného | 
| Datum_zahájení_předplatného | Datum začátku předplatného | 
| Datum ukončení předplatného | Datum konce předplatného | 
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
| PartnerAttributionType | Typ atribuce partnera | 
| SalesChannel | Kanál prodeje (Direct/CSP, Indirect/CSP, Direct a tak dále) | 
| ACR_USD | Výnosy spotřebované službou Azure (ACR) v amerických dolarech | 
| ID registrace | ID registrace předplatného Azure | 

### <a name="office-365-license-usage-report"></a>**Office 365 využití licencí**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenanta zákazníka | 
| CustomerTpid | ID nejvyššího nadřazeného zákazníka | 
| Název úlohy | Skype pro firmy, Teams, Exchange Online | 
| Month (Měsíc) | Měsíc, pro který se hlásí využití | 
| PaidAvailableUnits | Počet placených dostupných jednotek | 
| MonthlyActiveUsers | Počet měsíčních aktivních uživatelů | 
| CustomerName | Jméno zákazníka | 
| CustomerMarket | Zeměpisná poloha země na trhu zákazníka | 
| CustomerSegment | Segment zákazníka | 
| MPNId | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| PartnerLocation | Zeměpisné umístění partnera | 
| PartnerAttributionType | Typ přidělení partnera | 

### <a name="enterprise-mobility-license-usage-report"></a>**Enterprise Sestava využití licencí mobility**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenanta zákazníka | 
| CustomerTpid | Hlavní ID nadřazeného zákazníka | 
| Úloha úlohy | název úlohy Enterprise Mobility + Security (EMS) | 
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
| SubscriptionId | Identifikátor GUID předplatného | 
| SubscriptionStartDate | Počáteční datum předplatného | 
| SubscriptionEndDate | Datum ukončení předplatného | 
| SubscriptionStatus | Stav předplatného | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití | 
| RevSumDivisionName | Název dělení rev suma | 
| RevSumCategoryName | Název kategorie součtu rev | 
| SKU | SKU produktu | 
| SKUId | ID SKU produktu | 
| FreeVsPaidSKU | Označuje, zda se jedná o bezplatnou nebo placenou skladovou jednotku. | 
| SalesModel | Prodejní kanál, který se používá k prodeji předplatného | 
| DetailedSalesModel | Podrobný prodejní model předplatného | 
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
| DeploymentOpportunity | Aktuální příležitost nasazení | 
| ActiveUsagePercent | Aktuální procento využití v aktuálním prostředí | 

### <a name="power-bi-license-usage-report"></a>**Power BI sestava využití licencí**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| SubscriptionId | Identifikátor GUID předplatného | 
| SubscriptionStartDate | Počáteční datum předplatného | 
| SubscriptionEndDate | Datum ukončení předplatného | 
| SubscriptionStatus | Stav předplatného (aktivní, neaktivní nebo v období odkladu) | 
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
| AvailableSeats | Aktuální dostupná místa | 
| AssignedSeats | Aktuálně přiřazená místa | 
| ActiveSeats | Aktuální aktivní křesla | 
| DeploymentOpportunity | Aktuální příležitost nasazení | 
| ActiveUsagePercent | Aktuální procento využití v aktuálním prostředí | 

### <a name="teams-meetings-and-calls-report"></a>**sestava Teams schůzky a volání**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenanta zákazníka | 
| CustomerTpid | Identifikátor nejvyšší nadřazené položky zákazníka | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití | 
| Podúlohy | Podúlohy, pro které se nahlásí využití (schůzky, hovory nebo telefonní systémy) | 
| Počet schůzek | Počet schůzek | 
| Doba trvání schůzky | Celková doba trvání schůzky v hodinách | 

### <a name="teams-monthly-usage-report"></a>**sestava využití Teamsch měsíců**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenanta zákazníka | 
| CustomerTpid | Identifikátor nejvyšší nadřazené položky zákazníka | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití | 
| Podúlohy | Podúlohy, pro které se nahlásí využití (schůzky, hovory nebo telefonní systémy) | 
| Uživatelé klasické pracovní plochy | počet uživatelů, kteří používají Teams na ploše | 
| Mobilní uživatele | počet uživatelů, kteří používají Teams na mobilních zařízeních | 
| Webové uživatele | počet uživatelů, kteří používají Teams na webu | 
| AllUpParticipants | počet jedinečných uživatelů Teams za měsíc | 

### <a name="teams-usage-3p-apps-report"></a>**sestava 3P využití aplikací pro aplikace Teams**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenanta zákazníka | 
| CustomerTpid | Hlavní ID nadřazeného zákazníka | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití | 
| Název aplikace 3P | název aplikace Teams | 
| Počet uživatelů | Počet uživatelů pro aplikaci | 


### <a name="training-details-report"></a>**Sestava podrobností o školení**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| TrainingActivityId | Identifikátor školení | 
| TrainingTitle (Trénování názvu) | Název školení | 
| Typ trénování | Typ školení (certifikace nebo zkouška) | 
| Jednotlivý_název_první_položky | Jméno zákazníka | 
| IndividualLastName | Příjmení zákazníka | 
| E-mail | ID osobního e-mailu zákazníka | 
| CorpEmail | Office ID e-mailu zákazníka | 
| TrainingCompletionDate | Datum dokončení trénování | 
| Month (Měsíc) | Měsíc, pro který jsou data hlášena | 
| IcMCP | Určuje, jestli uživatel má certifikaci Microsoft Certified Professional (MCP). | 
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
| Název trénování | Název trénování | 
| Typ trénování | Typ školení (modul nebo studijní program) | 
| Produkty | Produkt, pro který je výukový modul použitelný | 
| Role | Příslušné role trénování | 
| Datum dokončení | Datum dokončení trénování | 
| ID MPN | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| Země | Zeměpisné umístění země partnera | 

### <a name="competency-summary-and-history-report"></a>**Souhrn kompetencí a sestava historie**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| Název kompetence | Název kompetence | 
| CompetencyLevel | Úroveň kompetence (gold nebo silver) | 
| Stav kompetence | Aktuální stav kompetence (Aktivní, Neaktivní nebo V období odkladu) | 
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
| SilverThreshold | Požadavek na výkon pro splnění silver competency | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Cloud Ascent – Microsoft 365 sestava sklonů**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ID MPN | Microsoft Partner Network ID | 
| Název partnera | Název partnera | 
| ID zákazníka | Číslo identifikátoru zákazníka | 
| Číslo DUNS | The Dun & Brad neschůdný (D&B) zákazníka, který má skóre z řad náchylnosti. | 
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
| PSČ | Poštovní směrovací číslo organizace | 
| Země | Zeměpisná poloha země organizace | 
| Segment | Segment trhu | 
| Dílčí segment | Segmentace trhu | 
| Shrnutí typu SMC | Typ SMC | 
| Hlavní nespravovaný – základ COMPUTE | Hlavní nespravované zákazníky – COMPUTE | 
| Hlavní nespravovaný – základ uživatele | Hlavní nespravované zákazníky – uživatel | 
| IsNonProfit | Indikuje, jestli je organizace nezisková (Ano nebo ne). | 
| Povolit vzdálenou pracovní Exchange Online cíl | zákazníci, kteří mají aktivní předplatné Exchange Online, přeprodat do Microsoft 365 | 
| Povolit vzdálenou práci – místní akvizici (aktuální verze) s licencemi pro PROPER v cloudu – + 10 | zákazník, který má stávající místní Office nebo Windows klienta. To znamená, že verze klienta je novější než verze konce životnosti (konce řádku). Zákazník má 10 nebo více licencí. Zákazník, který má skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní akvizici (aktuální verze) s licencemi pro PROPER v cloudu – <10 | zákazník, který má aktuální místní Office nebo klienta Windows (tj. verze novější než konce řádku). Zákazník má méně než 10 licencí. Zákazník, který má skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní pořízení (aktuální verze) bez licencí PROPER v cloudu – + 10 | zákazník, který má aktuální místní Office nebo klienta Windows (tj. verze novější než konce řádku). Zákazník má 10 nebo více licencí. Zákazník nemá skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní pořízení (aktuální verze) bez <10 licencí v cloudu | zákazník, který má aktuální místní Office nebo klienta Windows (tj. verze novější než konce řádku). Zákazník má méně než 10 licencí. Zákazník nemá skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní akvizici (konce řádku verzi) s licencemi pro procházím cloudovým properm – + 10 | zákazník, který má konce řádku místního Office nebo Windows klienta (tj. konce řádku verze nebo starší). Zákazník má 10 nebo více licencí. Zákazník má skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolení vzdálené práce v místním prostředí (konce řádku verze) s licencemi pro PROPER v cloudu – <10 | zákazník, který má konce řádku místního Office nebo Windows klienta (tj. konce řádku verze nebo starší). Zákazník má méně než 10 licencí. Zákazník má skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní pořízení (verze konce řádku) bez cloudových PROPER – + 10 licencí | zákazník, který má aktuální místní Office nebo klienta Windows (tj. verze konce řádku nebo starší). Zákazník má 10 nebo více licencí. Zákazník nemá skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní pořízení (konce řádku verze) bez cloudových PROPER – <10 | zákazník, který má aktuální místní Office nebo klienta Windows (tj. verze konce řádku nebo starší). Zákazník má méně než 10 licencí. Zákazník nemá skóre proper. Partner by měl cílit na Microsoft 365. | 
| povolit vzdálený pracovní postup s vysokou mírou prohlídky pro Microsoft 365 (Act NowithEvaluate) | Zákazník v potenciálním zákazníkovi s vysokou mírou PROPER pro Microsoft 365 | 
| Povolení vzdálené práce – soutěžování (přiblížení) s Microsoft 365 | zákazník s přiblížením a Microsoft 365 cílený na převod na Teams | 
| Povolit vzdálenou práci – soutěžit (Lupa) bez Microsoft 365 | Zákazník s přiblížením, cíl pro převod na Teams | 
| snižte náklady a spravujte-Microsoft 365 E3 cílené na Microsoft 365 E5 | stávající zákazník s Microsoft 365 E3, cíl pro Microsoft 365 E5 | 
| snižte náklady a spravujte – Microsoft 365 Business Basic a podnikové standardní zákazníky cílené na Microsoft 365 Business Premium | stávající zákazníci Microsoft 365 Business Basic a Business Standard, cíl pro Microsoft 365 Business Premium | 
| Transformace produktivity organizace – PROPER Surface | Zákazník zobrazuje PROPER pro plochu. | 
| M365Cluster | Identifikuje PROPER zákazníka k nákupu Microsoft 365. Zaměřte se na cíl a vyhodnoťte clustery, protože budou poskytovat vyšší výnosy. Informujte se o nurture a informujte zákazníky jenom v případě, že je stále dostupná kapacita a vyhodnoťte zákazníky. | 
| M365Fit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro naše nejlepší malé nebo střední firmy (SMB) k porovnání zákazníků a zjištění, zda se jedná o potenciální schopnost pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
| M365Intent | Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení pro definování clusterů. Bodování záměru se aktualizuje měsíčně. | 
| SurfaceCluster | Identifikuje náchylnost zákazníka k nákupu Surface tím, že konsoliduje doporučení Fit and Intent (Přizpůsobit a záměr) do clusteru. Zaměřte se teď na a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání jenom v případě, že existuje kapacita po provedení funkce Act Now a Evaluate customers are targeted(Vyhodnotit zákazníky). | 
| SurfaceFit | Interní a externí datové body, které definují pevné údaje. Bodování fitů používá k porovnání zákazníků podobný model pro naše nejlepší databáze, aby bylo možné porovnat zákazníky a zjistit, jestli se hodí pro cloudové produkty Microsoftu. Vyhodnocování fitů se aktualizuje čtvrtletně. | 
| SurfaceIntent | Signály související se sociálních sítěmi a online chováním zákazníka definují záměr. Skóre záměru je přeocené na fitu pro definování shluků. Bodování záměru se aktualizuje každý měsíc. | 
| O365Cluster | Identifikuje náchylnost zákazníka k nákupu Office 365. Zaměřte se teď na a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání jenom v případě, že existuje kapacita po provedení funkce Act Now a Evaluate customers are targeted(Vyhodnotit zákazníky). | 
| O365Fit | Interní a externí datové body, které definují pevné údaje. Bodování fitů používá k porovnání zákazníků podobný model pro naše nejlepší databáze, aby bylo možné porovnat zákazníky a zjistit, jestli se hodí pro cloudové produkty Microsoftu. Vyhodnocování fitů se aktualizuje čtvrtletně. | 
| O365Intent | Signály související se sociálních sítěmi a online chováním zákazníka definují záměr. Skóre záměru je přeocené na fitu pro definování shluků. Bodování záměru se aktualizuje každý měsíc. | 
| M365UpsellCustomer | Určuje, jestli se zákazníkovi zobrazuje kolísavost pro Microsoft 365 | 
| Má Google | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící produkty Google. | 
| Má AWS | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící Amazon Web Services (AWS). | 
| Má EA | Určuje, jestli je prodloužení smlouvou Enterprise (EA) nebo předplatným EA. | 
| Má otevřený | Určuje, jestli je prodloužení smlouvou Open Nebo Open Value. | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Ascent cloudu – sestava sklonů Dynamics 365**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ID MPN | Microsoft Partner Network (MPN) ID | 
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
| Nejspravované – výpočetní základ | Nejspravovaná zákazníci – výpočetní prostředky | 
| Nejspravované – uživatelská základna | Nejspravovaná zákazníci – uživatelé | 
| IsNonProfit | Určuje, jestli je organizace nezisková (Ano nebo Ne). | 
| Aktivace digitálního prodeje – Microsoft 365 – velikost >= 25 licencí (model s licencí SalesPro) | Zákazník bez Dynamics 365. Velikost místa: 25+. Partner by měl cílit na křížový prodej Dynamics 365 SalesPro. | 
| Aktivace digitálního prodeje – Dynamics 365 SalesPropensity (jednat hned nebo vyhodnotit) | Zákazníci s vysokou náchylností bez Dynamics 365. Partner by měl cílit na Dynamics 365 SalesPro. | 
| Řízení finančních rizik & podvodu – Místní instalační základna Dynamics – Navision (model náchylnosti k Business Central) | Stávající zákazník s místním Navision. Partner by měl cílit na Dynamics 365 Business Central. | 
| Správa finančních rizik & podvodu – Místní instalační základna Dynamics – Dynamics AX (model dynamics 365 Finance + Operations) | Stávající zákazník s místní osou AX Partner by měl cílit na Dynamics 365 Finance + Operations. | 
| Řízení finančních rizik & podvodu – Místní instalační základna Dynamics – Great Plains (model náchylnosti k Business Central) | Stávající zákazník s místními pláněmi Great Plains Partner by měl cílit na Dynamics 365 Business Central. | 
| Správa finančních rizik & podvody – Místní instalační základna Dynamics –Mon (model supenzity Business Central) | Stávající zákazník s místním předávkem Partner by měl cílit na Dynamics 365 Business Central. | 
| Správa finančních rizik & podvody – Místní instalační základna Dynamics – ostatní (model s návěsí Business Central) | Stávající zákazník s jinými místními řešeními, která tu ještě nejsou uvedená Partner by měl cílit na Dynamics 365 Business Central. | 
| Sestavování agilní obchodních procesů – místní instalační základna Dynamics – AX/GP/SL/NAV/Other (model dynamics 365 propensity) | Sestavování agilní obchodních procesů – místní instalační základna Dynamics – AX/GP/SL/NAV/Other (model dynamics 365 propensity) | 
| Sestavování agilní obchodních procesů – dynamics compete base – Mendix/OutSystems/Salesforce (model dynamics 365 propensity) | Sestavování agilní obchodních procesů – Dynamics compete base – Mendix/OutSystems/Salesforce (model dynamics 365 propensity) | 
| Sestavování agilní obchodních procesů – instalační základna Dynamics 365 Finance + Operations | Stávající zákazníci Dynamics 365 Finance + Operations Partner pro Power Apps. | 
| Sestavování agilní obchodních procesů – instalační základna Dynamics 365 Business Central | Stávající zákazníci Dynamics 365 Business Central Partner pro Power Apps. | 
| Sestavování agilní obchodních procesů – instalační základna Dynamics 365 Customer Engagement | Stávající zákazníci Dynamics 365 Customer Engagement Partner pro Power Apps. | 
| Vytvoření odolného dodavatelského řetězce – Windows a aktivace první úlohy Dynamics 365 jako správy dodavatelského řetězce Dynamics 365 u zákazníků, kteří nejsou oracle nebo SAP ERP (plánování podnikových zdrojů). | Cílí na zákazníky pro správu dodavatelského řetězce Dynamics 365 | 
| Vytvoření odolného dodavatelského řetězce – křížové prodáte Dynamics 365 Supply Chain Management a/nebo Retail or Commerce stávajícím zákazníkům Dynamics 365 Customer Engagement | Stávající zákazníci Dynamics 365 Customer Engagement, kteří se mají zaměřit na řízení dodavatelského řetězce Dynamics 365 napříč prodeji. | 
| Vytvoření odolného dodavatelského řetězce – křížové prodeje pro Dynamics 365 Supply Chain Management a/nebo Retail or Commerce do Dynamics 365 Customer Engagement a Oracle nebo SAP | Stávající zákazníci Dynamics 365 Customer Engagement s Oraclem nebo SAP cílí na správu dodavatelského řetězce Dynamics 365 | 
| D365BCCluster | Identifikuje náchylnost zákazníka k nákupu Dynamics 365 Business Central. Zákazníci, kteří zobrazují sklon pro Business Central, budou v kategoriích Střední a Malá. Zaměřte se teď na a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání pouze v případě, že existuje kapacita po cílení na zákazníky, kteří se vyhodnocují, a vyhodnoťte je. | 
| D365BCFit | Interní a externí datové body, které definují pevné údaje. Bodování fitů používá k porovnání zákazníků a určení, jestli jsou vhodné pro cloudové produkty Microsoftu, podobný model pro náš nejlepší protokol SMB. Vyhodnocování fitů se aktualizuje čtvrtletně. | 
| D365BCIntent | Signály související se sociálních sítěmi a online chováním zákazníka definují záměr. Skóre záměru je přeocené na fitu pro definování shluků. Bodování záměru se aktualizuje každý měsíc. | 
| D365FOCluster | Identifikuje náchylnost zákazníka k nákupu Dynamics 365 Finance and Operations. Zákazníci, kteří zobrazují sklony pro Finance + Operations, budou v horních nespravovaných kategoriích. Zaměřte se teď na a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání pouze v případě, že existuje kapacita po cílení na zákazníky, kteří se vyhodnocují, a vyhodnoťte je. | 
| D365FOFit | Interní a externí datové body, které definují pevné údaje. Bodování fitů používá k porovnání zákazníků a určení, jestli jsou vhodné pro cloudové produkty Microsoftu, podobný model pro náš nejlepší protokol SMB. Vyhodnocování fitů se aktualizuje čtvrtletně. | 
| D365FOIntent | Signály související se sociálních sítěmi a online chováním zákazníka definují záměr. Skóre záměru je přeocené na fitu pro definování shluků. Bodování záměru se aktualizuje každý měsíc. | 
| D365CECluster | Identifikuje náchylnost zákazníka k nákupu Dynamics 365 Customer Engagement. Zákazníci, kteří zobrazují sklony pro Customer Engagement, budou v kategoriích Střední a Malá. Zaměřte se teď na a vyhodnoťte clustery, protože budou mít vyšší výnos. Cílení zákazníků na rozvoj a vzdělávání pouze v případě, že existuje kapacita po cílení na zákazníky, kteří se vyhodnocují, a vyhodnoťte je. | 
| D365CEFit | Označuje Fit for Dynamics 365 Customer Engagement. | 
| D365CEIntent | Označuje záměr pro Dynamics 365 Customer Engagement. | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Určuje, jestli má zákazník otevřené prodloužení pro místní DYNAMICS AX nebo CRM. | 
| M365UpsellCustomer | Určuje, jestli se zákazníkovi zobrazuje kolísavost pro Microsoft 365 | 
| Má Google | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící produkty Google. | 
| Má AWS | Určuje, jestli zákazník vykazuje konkurenční signály pro vlastnící produkty AWS. | 
| Má EA | Určuje, jestli je prodloužení předplatného EA nebo EA. | 
| Má otevřený | Určuje, jestli je prodloužení smlouvou Open Nebo Open Value. | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud Ascent – sestava náchylnosti k Azure**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ID MPN | Microsoft Partner Network (MPN) ID | 
| Název partnera | Název partnera | 
| ID zákazníka | Číslo identifikátoru zákazníka | 
| Číslo DUNS | The Dun & Brad number of the customer who's scored for propensity | 
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
| PSČ | Poštovní směrovací číslo organizace | 
| Země | Zeměpisná poloha země | 
| Segment | Segment trhu | 
| Dílčí segment | Segmentace trhu | 
| Shrnutí typu SMC | Typ SMC | 
| Hlavní nespravovaný – základ COMPUTE | Hlavní nespravované zákazníky – COMPUTE | 
| Hlavní nespravovaný – základ uživatele | Hlavní nespravované zákazníky – uživatelé | 
| IsNonProfit | Indikuje, jestli je organizace nezisková (Ano nebo ne). | 
| migrace – konce řádku Windows server-konce řádku Windows server IB s promi v cloudu proper – 5 a licence | zákazník, který má konce řádku místní Windows Server (tj. konce řádku verze nebo starší). Zákazník má 5 nebo více licencí. Zákazník, který má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – konce řádku Windows server-konce řádku Windows server IB s použitím proch proper v cloudu – <5 | zákazník, který má konce řádku místní Windows Server (tj. konce řádku verze nebo starší). Zákazník má méně než 5 licencí. Zákazník, který má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – konce řádku Windows server-konce řádku Windows server IB bez proch proper v cloudu – 5 a licence | zákazník, který má konce řádku místní Windows Server (tj. konce řádku verze nebo starší). Zákazník má více než 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – konce řádku Windows server-konce řádku Windows server IB bez proch proper v cloudu – <5 licencí | zákazník, který má konce řádku místní Windows Server (tj. konce řádku verze nebo starší). Má méně než 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – konce řádku SQL-SQL Server konce řádku a bez cloudového proper – 5 a licence | zákazník, který má konce řádku místní SQL Server (tj. konce řádku verze nebo starší). Zákazník má 5 licencí. Zákazník má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – konce řádku SQL-konce řádku a s SQL Server IB s promi proper – <5 licencí | zákazník, který má konce řádku místní SQL Server (tj. konce řádku verze nebo starší). Má méně než 5 licencí. Zákazník, který má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – konce řádku SQL-SQL Server konce řádku a bez cloudového proper – 5 a licence | zákazník, který má konce řádku místní SQL Server (tj. konce řádku verze nebo starší). Zákazník má 5 nebo více licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – konce řádku SQL-SQL Server konce řádku a bez cloudového proper – <5 licencí | zákazník, který má konce řádku místní SQL Server (tj. konce řádku verze nebo starší). Zákazník má méně než 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – migrace místního Windows serveru – aktuální Windows server IB s procházími propermi v cloudu – 5 + licence | zákazník, který má aktuální místní Windows Server (tj. verze novější než konce řádku). Zákazník má 5 licencí. Zákazník má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – migrace místního Windows serveru – aktuální Windows server IB s procházími propermi v cloudu – <5 | zákazník, který má aktuální místní Windows Server (tj. verze novější než konce řádku). Zákazník má méně než 5 licencí. Zákazník má skóre PROPER pro Azure. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – migrace místního Windows serveru – aktuální Windows server IB bez použití proper v cloudu – 5 a licence | zákazník, který má aktuální místní Windows Server (tj. verze novější než konce řádku). Zákazník má 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – migrace místního Windows serveru – aktuální Windows server IB bez použití proper v cloudu – <5 | zákazník, který má aktuální místní Windows Server (tj. verze novější než konce řádku). Zákazník má méně než 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – migrace do Azure SQL nebo SQL virtuálních počítačů (vm) – aktuální SQL Server IB s použitím proper v cloudu – 5 a licence | zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má 5 licencí. Zákazník má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – migrace do Azure SQL nebo SQL virtuálních počítačů – aktuální SQL Server IB s použitím proper v cloudu – <5 – licence | zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má méně než 5 licencí. Zákazník má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – migrace do Azure SQL nebo SQL virtuálních počítačů – aktuální SQL Server IB bez proper v cloudu – 5 a licence | zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – migrace do Azure SQL nebo SQL virtuálních počítačů – aktuální SQL Server IB bez použití proper v cloudu – <5 licencí | zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má méně než 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – OSS – migrace do Open Source Shakespeare (OSS) DB | Stávající zákazník s některým z následujících konkurenčních produktů: PostgreSQL, MySQL, MariaDB. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – OSS-Linux v Azure | Stávající zákazník se systémem Linux. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – SAP-SAP v Azure | Stávající zákazník se SAP. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – Windows virtuální plocha – vzdálená plocha IB | identifikuje zákazníky se službou vzdálená plocha služby active Windows. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| migrace – Windows virtuální plochy – moderní práce v různých prodejích do Azure/WVD | identifikuje zákazníky s Microsoft 365 a nemá Azure. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – VMware IB | Stávající zákazník s produktem: VMware. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – Citrix IB | Stávající zákazník s produktem: systémy Citrix. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| inovace – analýza-Power BI IB s vysokou mírou proper Azure | zákazníci s předplatným a aktivním Power BI, včetně: Power BI-Standalone Pro, Power BI sady Azure, Power BIch Officech sad, Power BIch sad – Microsoft 365 | 
| Enable-DevOps s GitHub-Visual Studio/MSDN IB | identifikuje zákazníky s aktivními Visual Studio verzemi. | 
| Windows Standardní verze serveru | zobrazí verzi Windows nákupy serveru na úrovni standard zákazníkem. | 
| Windows Licence na Server Standard | zobrazuje typ licence pro nákupy Windows serveru na úrovni standard zákazníkem. | 
| Windows Verze datového centra serveru | zobrazuje verzi Windows nákupu datového centra zákazníkem. | 
| Windows Licence k datovému centru serveru | zobrazuje typ licence Windows nákupu datového centra od zákazníka. | 
| AzureFit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro náš nejlepší protokol SMB pro porovnání zákazníků a zjištění, jestli jsou potenciálními možnostmi pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
| AzureIntent | Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení pro definování clusterů. Bodování záměru se aktualizuje měsíčně. | 
| AzureCluster | Slouží k identifikaci per zákazníka k nákupu Azure tím, že se do clusteru konsolidují doporučení k přizpůsobení a záměru. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| WindowsServerDataCenter_HasOpenRenewal | určuje, jestli má zákazník otevřené obnovení pro Datacenter Windows serveru. | 
| WindowsServerStandard_HasOpenRenewal | určuje, jestli má zákazník otevřené obnovení pro Windows Server Standard. | 
| AzureUpsellCustomer | Určuje, jestli zákazník zobrazuje přeprodat PROPER pro Azure. | 
| Má Google | Určuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnictví produktů Google. | 
| Má AWS | Určuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnící AWS produkty. | 
| Má EA | Určuje, jestli je obnovení předplatného EA nebo EA. | 
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
| Země | Zeměpisná poloha země | 
| Segment | Segment trhu | 
| Dílčí segment | Segmentace trhu | 
| Shrnutí typu SMC | Typ SMC | 
| Hlavní nespravovaný – základ COMPUTE | Hlavní nespravované zákazníky – COMPUTE | 
| Hlavní nespravovaný – základ uživatele | Hlavní nespravované zákazníky – uživatelé | 
| IsNonProfit | Indikuje, jestli je organizace nezisková (Ano nebo ne). | 
| Má Google | Určuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnící AWS produkty. | 
| Má AWS | Určuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnící AWS produkty. | 
| Cluster Azure | Identifikuje PROPER zákazníka k nákupu Azure. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| D365 finance + provozní cluster | Identifikuje PROPER zákazníka k nákupu Dynamics 365 finance a operací. Zákazníci, kteří zobrazují PROPER pro finance a operace, budou v hlavních nespravovaných kategoriích. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| Cluster D365 CE | Identifikuje PROPER zákazníka k nákupu zákaznického zapojení Dynamics 365. Zákazníci, kteří zobrazují PROPER pro zapojení zákazníka, budou ve středních a malých kategoriích. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| Cluster D365 BC | Identifikuje PROPER zákazníka k nákupu Dynamics 365 Business Central. Zákazníci, kteří zobrazují PROPER pro firmu Business Central, budou mít střední a malou kategorii. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| Microsoft 365 Služby | Identifikuje PROPER zákazníka k nákupu Microsoft 365. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| Licenční program | Identifikuje typ licenčního programu pro obnovení. | 
| ID smlouvy | Identifikátor smlouvy | 
| Koncové datum smlouvy | Koncové datum smlouvy | 
| Typ vypršení platnosti | Typ vypršení platnosti | 
| Vypršení výnosů | Tržby přidružené k vypršení platnosti předplatných | 
| Má EA | Určuje, jestli je obnovení předplatného EA nebo EA. | 
| Má otevřené | Určuje, jestli je obnovování smlouva otevřené nebo otevřené hodnoty. | 
| Zákazník Azure přeprodat | Určuje, jestli zákazník zobrazuje přeprodat PROPER pro Azure. | 
| Microsoft 365 Zákazník přeprodat | Určuje, jestli zákazník zobrazuje přeprodat PROPER pro Microsoft 365. | 
| RevSumDivisionName | Identifikuje produkt, který je až pro obnovení. | 

## <a name="next-steps"></a>Další kroky

Další informace najdete v tématu [stažení sestav](insights-download-reports.md).
