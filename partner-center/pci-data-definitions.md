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
ms.openlocfilehash: 427ca3b60ec527a6a371a232538647448d03b084
ms.sourcegitcommit: 6632d7452be36010bfc8c6823efe5a5197377989
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/27/2021
ms.locfileid: "98861389"
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
| Country (Země) | Umístění země partnera | 
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
| Product | Produkt prodal zákazník od MPN: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI nebo Microsoft Azure | 
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
> Data o výnosech a ACR jsou k dispozici pouze uživatelům, kteří jsou správci sestav od manažera.

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ResellerMPNid | Identifikátor Microsoft Partner Network prodejce | 
| ResellerName | Jméno prodejce | 
| ResellerMarket | Prodejce země na trhu | 
| IndirectProviderMPNId | Identifikátor Microsoft Partner Network nepřímého zprostředkovatele | 
| IndirectProviderName | Název nepřímého zprostředkovatele | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití a výnosy | 
| Product | Název produktu | 
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
| Product | Produkt prodávaný partnerem pro zákazníky | 
| SKU | SKU produktu | 
| MPNId | ID Microsoft Partner Network partnera | 
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

### <a name="teams-meetings-and-calls-report"></a>**Sestavy schůzek a volání týmů**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenanta zákazníka | 
| CustomerTpid | Identifikátor nejvyšší nadřazené položky zákazníka | 
| Month (Měsíc) | Měsíc, pro který se nahlásí využití | 
| Podúlohy | Podúlohy, pro které se nahlásí využití (schůzky, hovory nebo telefonní systémy) | 
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
| CorpEmail | ID e-mailu pro Office zákazníka | 
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
| TrainingType | Typ školení (modul nebo vzdělávací cesta) | 
| Produkty | Produkt, na který se vztahuje modul učení | 
| Role | Příslušné role školení | 
| CompletionDate | Datum dokončení školení | 
| MPNId | Identifikátor Microsoft Partner Network | 
| PartnerName | Název partnera | 
| Country (Země) | Zeměpisná poloha země partnera | 

### <a name="competency-summary-and-history-report"></a>**Souhrn kompetencí a sestava historie**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| CompetencyName | Název kompetence | 
| CompetencyLevel | Úroveň kompetence (zlatá nebo stříbrná) | 
| CompetencyStatus | Aktuální stav kompetence (aktivní, neaktivní nebo v období odkladu) | 
| CompetencyStartDate | Počáteční datum kompetence | 
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

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Sestava o proMicrosoft 365ch properch v cloudu**

| Název sloupce | Popis dat | 
| :--------- | :--------- | 
| ID MPN | ID Microsoft Partner Network | 
| Název partnera | Název partnera | 
| ID zákazníka | Číslo identifikátoru zákazníka | 
| DUNS číslo | Telefonické připojení & Bradstreet (D&B) číslo zákazníka, u kterého se má vyhodnocovat hodnocení Proper | 
| Název účtu | Název účtu | 
| Doména | Doména účtu | 
| Velikost organizace | Velikost organizace | 
| Obor | Odvětví, do kterého organizace patří | 
| Svisle | Svislá část zákazníka, u kterého se skóre v rámci PROPER identifikovali podle identifikace od Microsoftu, D&B a dalších oborových standardů | 
| Plošný | Zeměpisná oblast umístění | 
| Pobočka | Dceřiná společnost zákazníka, u kterého se má skóre na Proper | 
| Sales Territory (Prodejní oblast) | Prodejní teritorium zákazníka, u kterého se provádí hodnocení Proper | 
| City (Město) | Zeměpisná poloha města organizace | 
| State | Zeměpisné umístění organizace | 
| PSČ | Poštovní směrovací číslo organizace | 
| Country (Země) | Zeměpisná poloha země organizace | 
| Segment | Segment trhu | 
| Dílčí segment | Segmentace trhu | 
| Shrnutí typu SMC | Typ SMC | 
| Hlavní nespravovaný – základ COMPUTE | Hlavní nespravované zákazníky – COMPUTE | 
| Hlavní nespravovaný – základ uživatele | Hlavní nespravované zákazníky – uživatel | 
| IsNonProfit | Indikuje, jestli je organizace nezisková (Ano nebo ne). | 
| Povolit vzdálený pracovní cíl Exchange Online | Zákazníci, kteří mají aktivní předplatné Exchange Online, přeprodat Microsoft 365 | 
| Povolit vzdálenou práci – místní akvizici (aktuální verze) s licencemi pro PROPER v cloudu – + 10 | Zákazníka, který má stávajícího místního Office nebo klienta Windows. To znamená, že verze klienta je novější než verze konce životnosti (konce řádku). Zákazník má 10 nebo více licencí. Zákazník, který má skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní akvizici (aktuální verze) s licencemi pro PROPER v cloudu – <10 | Zákazník, který má stávajícího místního Office nebo klienta Windows (tj. verze novější než konce řádku). Zákazník má méně než 10 licencí. Zákazník, který má skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní pořízení (aktuální verze) bez licencí PROPER v cloudu – + 10 | Zákazník, který má stávajícího místního Office nebo klienta Windows (tj. verze novější než konce řádku). Zákazník má 10 nebo více licencí. Zákazník nemá skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní pořízení (aktuální verze) bez <10 licencí v cloudu | Zákazník, který má stávajícího místního Office nebo klienta Windows (tj. verze novější než konce řádku). Zákazník má méně než 10 licencí. Zákazník nemá skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní akvizici (konce řádku verzi) s licencemi pro procházím cloudovým properm – + 10 | Zákazník, který má konce řádku místního Office nebo klienta Windows (to znamená, že konce řádku verze nebo starší). Zákazník má 10 nebo více licencí. Zákazník má skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolení vzdálené práce v místním prostředí (konce řádku verze) s licencemi pro PROPER v cloudu – <10 | Zákazník, který má konce řádku místního Office nebo klienta Windows (to znamená, že konce řádku verze nebo starší). Zákazník má méně než 10 licencí. Zákazník má skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní pořízení (verze konce řádku) bez cloudových PROPER – + 10 licencí | Zákazník, který má stávajícího místního Office nebo klienta Windows (tj. verze konce řádku nebo starší). Zákazník má 10 nebo více licencí. Zákazník nemá skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálenou práci – místní pořízení (konce řádku verze) bez cloudových PROPER – <10 | Zákazník, který má stávajícího místního Office nebo klienta Windows (tj. verze konce řádku nebo starší). Zákazník má méně než 10 licencí. Zákazník nemá skóre proper. Partner by měl cílit na Microsoft 365. | 
| Povolit vzdálený pracovní postup s vysokou mírou prohlídky pro Microsoft 365 (ACT NowithEvaluate) | Zákazník v potenciálním zákazníkovi s vysokou mírou PROPER pro Microsoft 365 | 
| Povolení vzdálené práce – soutěžování (přiblížení) s Microsoft 365 | Zákazník s přiblížením a Microsoft 365 cíli pro převod na týmy | 
| Povolit vzdálenou práci – soutěžit (Lupa) bez Microsoft 365 | Zákazník s přiblížením, cíl pro převod na týmy | 
| Snížení nákladů a Správa – Microsoft 365 E3 cílené pro Microsoft 365 E5 | Stávající zákazník s Microsoft 365 E3, cíl pro Microsoft 365 E5 | 
| Snižte náklady a spravujte Microsoft 365 Business zákazníky v jazyce Basic a Business Standard, které cílí na Microsoft 365 Business Premium. | Stávající zákazníci Microsoft 365 Business Basic a Business Standard, cíl pro Microsoft 365 Business Premium | 
| Transformace produktivity organizace – PROPER Surface | Zákazník zobrazuje PROPER pro plochu. | 
| M365Cluster | Identifikuje PROPER zákazníka k nákupu Microsoft 365. Zaměřte se na cíl a vyhodnoťte clustery, protože budou poskytovat vyšší výnosy. Informujte se o nurture a informujte zákazníky jenom v případě, že je stále dostupná kapacita a vyhodnoťte zákazníky. | 
| M365Fit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro naše nejlepší malé nebo střední firmy (SMB) k porovnání zákazníků a zjištění, zda se jedná o potenciální schopnost pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
| M365Intent | Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení pro definování clusterů. Bodování záměru se aktualizuje měsíčně. | 
| SurfaceCluster | Slouží k identifikaci PROPER zákazníka k nákupu povrchu tím, že se do clusteru konsolidují doporučení k přizpůsobení a záměrům. Zaměřte se na cíl a vyhodnoťte clustery, protože budou poskytovat vyšší výnosy. Informujte se o nurture a informujte zákazníky jenom v případě, že je stále dostupná kapacita a vyhodnoťte zákazníky. | 
| SurfaceFit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro naše nejlepší SMB k porovnání zákazníků a zjištění, jestli jsou potenciálními produkty pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
| SurfaceIntent | Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení pro definování clusterů. Bodování záměru se aktualizuje měsíčně. | 
| O365Cluster | Identifikuje PROPER zákazníka k nákupu Office 365. Zaměřte se na cíl a vyhodnoťte clustery, protože budou poskytovat vyšší výnosy. Informujte se o nurture a informujte zákazníky jenom v případě, že je stále dostupná kapacita a vyhodnoťte zákazníky. | 
| O365Fit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro naše nejlepší SMB k porovnání zákazníků a zjištění, jestli jsou potenciálními produkty pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
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
| DUNS číslo | Telefonické připojení & Bradstreet číslo zákazníka, který je v hodnocení pro Proper | 
| Název účtu | Název účtu | 
| Doména | Doména účtu | 
| Velikost organizace | Velikost organizace | 
| Obor | Odvětví, do kterého organizace patří | 
| Svisle | Svislá část zákazníka, u kterého se skóre v rámci PROPER identifikovali podle identifikace od Microsoftu, D&B a dalších oborových standardů
| Plošný | Zeměpisná oblast umístění | 
| Pobočka | Dceřiná společnost zákazníka, u kterého se má skóre na Proper | 
| Sales Territory (Prodejní oblast) | Prodejní teritorium zákazníka, u kterého se provádí hodnocení Proper | 
| City (Město) | Zeměpisná poloha města | 
| State | Zeměpisné umístění stavu | 
| PSČ | Poštovní směrovací číslo organizace | 
| Country (Země) | Zeměpisná poloha země | 
| Segment | Segment trhu | 
| Dílčí segment | Segmentace trhu | 
| Shrnutí typu SMC | Kategorizace zákazníka: hlavní nespravované uživatelské základy jsou zákazníky, kteří mají více než 300 zaměstnanců, hlavní nespravované výpočetní základy jsou zákazníci s USD10em, 3000 v rámci Azure tři roky jsou zákazníky s 25 zaměstnanci nebo vyšší a malým firmám jsou zákazníci s méně než 25 zaměstnanci. | 
| Hlavní nespravovaný – základ COMPUTE | Hlavní nespravované zákazníky – COMPUTE | 
| Hlavní nespravovaný – základ uživatele | Hlavní nespravované zákazníky – uživatelé | 
| IsNonProfit | Indikuje, jestli je organizace nezisková (Ano nebo ne). | 
| Aktivace digitálního prodeje-Microsoft 365-velikost sedadel >= 25 míst (model PROPER SalesPro) | Zákazník bez Dynamics 365. Velikost sedadla: 25 +. Partner by měl cílit na prodej Dynamics 365 SalesPro. | 
| Aktivace digitálního prodeje – Dynamics 365 SalesPro Proper (ACT nyní nebo Evaluate) | Zákazníci s vysokou mírou PROPER bez Dynamics 365. Partner by měl cílit na Dynamics 365 SalesPro. | 
| Správa finančních rizik & podvodů v místním prostředí – Dynamics – instalace pro základnu – Navision (model centrálních per pro firmy) | Stávající zákazník s místním Navision. Partner by měl cílit na Dynamics 365 Business Central. | 
| Správa finančních rizik & podvodů – místní instalace aplikace Dynamics AX – základní – Dynamics 365 (model PROPER Dynamics finance + operace) | Stávající zákazník s místní službou AX. Partner by měl cílit na operace Dynamics 365 finance +. | 
| Správa finančních rizik & podvodů v místním prostředí – místní instalace – velká místa (model centrálních per pro firmy) | Stávající zákazník s místními skvělými Plains. Partner by měl cílit na Dynamics 365 Business Central. | 
| Správa finančních rizik & podvodů – místní instalace aplikace Dynamics Solomon (model centrálních per pro firmy) | Stávající zákazník s místní Šalamounovy ostrovy Partner by měl cílit na Dynamics 365 Business Central. | 
| Správa finančních rizik & podvodů v místním prostředí – místní instalace (model centrálních per pro firmy) | Stávající zákazník s dalšími místními řešeními, která ještě nejsou v seznamu uvedená. Partner by měl cílit na Dynamics 365 Business Central. | 
| Sestavování agilních podnikových procesů – Dynamics – místní instalace – základní – AX/GP/SL/NAV/ostatní (model PROPER Dynamics 365) | Sestavování agilních podnikových procesů – Dynamics – místní instalace – základní – AX/GP/SL/NAV/ostatní (model PROPER Dynamics 365) | 
| Vytváření agilních obchodních procesů – Dynamics konkurenční báze – Mendix/subsystéms/Salesforce (model PROPER Dynamics 365) | Vytváření agilních obchodních procesů – Dynamics konkurenční báze – Mendix/subsystéms/Salesforce (model PROPER Dynamics 365) | 
| Vytváření agilních obchodních procesů – základ pro Dynamics 365 finance + Operations Install | Stávající zákazníci s Dynamics 365 financemi a provozními operacemi. Partner pro cílení Power Apps. | 
| Sestavování agilních obchodních procesů – základ instalace Dynamics 365 Business Central | Stávající zákazníci s obchodním ústředním odvětvím Dynamics 365. Partner pro cílení Power Apps. | 
| Vytváření agilních obchodních procesů – základ pro instalaci Dynamics 365 Customer Engagement | Stávající zákazníci Dynamics 365 Customer Engagement. Partner pro cílení Power Apps. | 
| Sestavte odolný dodavatelský řetězec – Windows a aktivujte první úlohu Dynamics 365 jako správu dodavatelských řetězců Dynamics 365 s zákazníky, kteří nepoužívají Oracle nebo SAP ERP (Enterprise Resource Planning). | Cílové zákazníky pro správu dodavatelských řetězců Dynamics 365 | 
| Sestavení odolného dodavatelského řetězce – meziprodejní Správa dodavatelských řetězců v Dynamics 365 a maloobchodu nebo obchodování s existujícími zákazníky Dynamics 365 Customer Engagement | Stávající zákazníci Dynamics 365 Customer Engagement cílí na spolupráci s prodejem dodavatelských dodavatelských řetězců v sadě Dynamics 365. | 
| Sestavení odolného dodavatelského řetězce – meziprodejní Správa dodavatelských řetězců v Dynamics 365 a maloobchod nebo prodej do Dynamics 365 Customer Engagement a Oracle nebo SAP | Stávající zákazníci Dynamics 365 Customer Engagement s Oracle nebo SAP pro cílení na správu dodavatelských řetězců Dynamics 365 | 
| D365BCCluster | Identifikuje PROPER zákazníka k nákupu Dynamics 365 Business Central. Zákazníci, kteří zobrazují PROPER pro firmu Business Central, budou mít střední a malou kategorii. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| D365BCFit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro náš nejlepší protokol SMB pro porovnání zákazníků a zjištění, jestli jsou potenciálními možnostmi pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
| D365BCIntent | Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení pro definování clusterů. Bodování záměru se aktualizuje měsíčně. | 
| D365FOCluster | Identifikuje PROPER zákazníka k nákupu Dynamics 365 finance a operací. Zákazníci, kteří zobrazují PROPER pro finance a operace, budou v hlavních nespravovaných kategoriích. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| D365FOFit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro náš nejlepší protokol SMB pro porovnání zákazníků a zjištění, jestli jsou potenciálními možnostmi pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
| D365FOIntent | Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení pro definování clusterů. Bodování záměru se aktualizuje měsíčně. | 
| D365CECluster | Identifikuje PROPER zákazníka k nákupu zákaznického zapojení Dynamics 365. Zákazníci, kteří zobrazují PROPER pro zapojení zákazníka, budou ve středních a malých kategoriích. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| D365CEFit | Indikuje přizpůsobení pro zákaznickou zapojení Dynamics 365. | 
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
| DUNS číslo | Telefonické připojení & Bradstreet číslo zákazníka, který je v hodnocení pro Proper | 
| Název účtu | Název účtu | 
| Doména | Doména účtu | 
| Velikost organizace | Velikost organizace | 
| Obor | Obor | 
| Svisle | Svislá část zákazníka, u kterého se skóre v rámci PROPER identifikovali podle identifikace od Microsoftu, D&B a dalších oborových standardů | 
| Plošný | Zeměpisná oblast umístění | 
| Pobočka | Dceřiná společnost zákazníka, u kterého se má skóre na Proper | 
| Sales Territory (Prodejní oblast) | Prodejní teritorium zákazníka, u kterého se provádí hodnocení Proper | 
| City (Město) | Zeměpisná poloha města | 
| State | Zeměpisné umístění stavu | 
| PSČ | Poštovní směrovací číslo organizace | 
| Country (Země) | Zeměpisná poloha země | 
| Segment | Segment trhu | 
| Dílčí segment | Segmentace trhu | 
| Shrnutí typu SMC | Typ SMC | 
| Hlavní nespravovaný – základ COMPUTE | Hlavní nespravované zákazníky – COMPUTE | 
| Hlavní nespravovaný – základ uživatele | Hlavní nespravované zákazníky – uživatelé | 
| IsNonProfit | Indikuje, jestli je organizace nezisková (Ano nebo ne). | 
| Migrace – konce řádku Windows serveru – konce řádku Windows serveru IB s Promi v cloudu PROPER – 5 a licence | Zákazník, který má konce řádku místní Windows Server (tj. konce řádku verze nebo starší). Zákazník má 5 nebo více licencí. Zákazník, který má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – konce řádku Windows serveru – konce řádku Windows serveru IB s použitím PROPER v cloudu – <5 – licence | Zákazník, který má konce řádku místní Windows Server (tj. konce řádku verze nebo starší). Zákazník má méně než 5 licencí. Zákazník, který má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – konce řádku Windows serveru – konce řádku Windows serveru IB bez Proch PROPER v cloudu – 5 a licence | Zákazník, který má konce řádku místní Windows Server (tj. konce řádku verze nebo starší). Zákazník má více než 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – konce řádku Windows serveru – konce řádku Windows serveru IB bez Proch PROPER v cloudu – licence <5 | Zákazník, který má konce řádku místní Windows Server (tj. konce řádku verze nebo starší). Má méně než 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – konce řádku SQL-konce řádku SQL Server IB s Promi cloudových PROPER – 5 a licence | Zákazník, který má konce řádku místní SQL Server (tj. konce řádku verze nebo starší). Zákazník má 5 licencí. Zákazník má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – konce řádku SQL-konce řádku SQL Server IB a u cloudových PROPER – <5 licencí | Zákazník, který má konce řádku místní SQL Server (tj. konce řádku verze nebo starší). Má méně než 5 licencí. Zákazník, který má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – konce řádku SQL-konce řádku SQL Server IB bez použití PROPER v cloudu – 5 a licence | Zákazník, který má konce řádku místní SQL Server (tj. konce řádku verze nebo starší). Zákazník má 5 nebo více licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – konce řádku SQL-konce řádku SQL Server IB bez použití PROPER v cloudu – <5 licencí | Zákazník, který má konce řádku místní SQL Server (tj. konce řádku verze nebo starší). Zákazník má méně než 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace místního Windows serveru – aktuální Windows Server IB s procházími propermi v cloudu – 5 a licence | Zákazník, který má aktuální místní Windows Server (tj. verze novější než konce řádku). Zákazník má 5 licencí. Zákazník má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace místního Windows serveru – aktuální Windows Server IB s použitím PROPER v cloudu – <5 – licence | Zákazník, který má aktuální místní Windows Server (tj. verze novější než konce řádku). Zákazník má méně než 5 licencí. Zákazník má skóre PROPER pro Azure. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace místního Windows serveru – aktuální Windows Server IB bez cloudové PROPER – 5 a licence | Zákazník, který má aktuální místní Windows Server (tj. verze novější než konce řádku). Zákazník má 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace místního Windows serveru – aktuální Windows Server IB bez <ch PROPER v cloudu – licence – 5 | Zákazník, který má aktuální místní Windows Server (tj. verze novější než konce řádku). Zákazník má méně než 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace na virtuální počítače Azure SQL nebo SQL (VM) – aktuální SQL Server i s u cloudových PROPER – 5 a licence | Zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má 5 licencí. Zákazník má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace na virtuální počítače Azure SQL nebo SQL – aktuální SQL Server IB s použitím PROPER v cloudu – <5 | Zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má méně než 5 licencí. Zákazník má skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace na virtuální počítače Azure SQL nebo SQL – aktuální SQL Server IB bez použití PROPER v cloudu – 5 a licence | Zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – migrace na virtuální počítače Azure SQL nebo SQL – aktuální SQL Server IB bez použití PROPER v cloudu – <5 | Zákazník, který má aktuální místní SQL Server (tj. verze novější než konce řádku). Zákazník má méně než 5 licencí. Zákazník nemá skóre proper. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – OSS – migrace do Open Source Shakespeare (OSS) DB | Stávající zákazník s některým z následujících konkurenčních produktů: PostgreSQL, MySQL, MariaDB. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – OSS-Linux v Azure | Stávající zákazník se systémem Linux. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – SAP-SAP v Azure | Stávající zákazník se SAP. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – Windows Virtual Desktop – Vzdálená plocha – IB | Identifikuje zákazníky s aktivní službou Vzdálená plocha systému Windows. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – Windows Virtual Desktop – moderní práce v různých prodejích do Azure/WVD | Identifikuje zákazníky s Microsoft 365 a nemá Azure. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – VMware IB | Stávající zákazník s produktem: VMware. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Migrace – Citrix IB | Stávající zákazník s produktem: systémy Citrix. Partner by měl cílit tohoto zákazníka na migraci do Azure. | 
| Inovace – analýza-Power BI IB s vysokou mírou PROPER Azure | Zákazníci s předplatným a aktivním Power BI, včetně: Power BI-Standalone pro, Power BI – sady pro Azure, sady Power BI sady Office, Power BI sady – Microsoft 365 | 
| Enable-DevOps s GitHubem – Visual Studio/MSDN IB | Identifikuje zákazníky s aktivními verzemi sady Visual Studio. | 
| Windows Server Standard verze | Zobrazuje verzi nákupů Windows serveru Standard podle zákazníka. | 
| Windows Server Standard License | Zobrazí typ licence pro nákupy Windows serveru Standard podle zákazníka. | 
| Verze datového centra Windows serveru | Zobrazuje verzi Windows Data Center nákupů podle zákazníka. | 
| Licence datového centra Windows serveru | Zobrazí typ licence pro nákup datového centra Windows podle zákazníka. | 
| AzureFit | Interní a externí datové body, které definují firmographics. Vyhodnocování přizpůsobení používá lookalike model pro náš nejlepší protokol SMB pro porovnání zákazníků a zjištění, jestli jsou potenciálními možnostmi pro cloudové produkty Microsoftu. Vyhodnocování podle skóre se aktualizuje čtvrtletně. | 
| AzureIntent | Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení pro definování clusterů. Bodování záměru se aktualizuje měsíčně. | 
| AzureCluster | Slouží k identifikaci per zákazníka k nákupu Azure tím, že se do clusteru konsolidují doporučení k přizpůsobení a záměru. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| WindowsServerDataCenter_HasOpenRenewal | Určuje, jestli má zákazník otevřené obnovení pro datacenter Windows serveru. | 
| WindowsServerStandard_HasOpenRenewal | Určuje, jestli má zákazník otevřené obnovení pro Windows Server Standard. | 
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
| Název účtu | Název účtu | 
| Doména | Doména účtu | 
| Velikost organizace | Velikost organizace | 
| Obor | Obor | 
| Svisle | Svislá část zákazníka, u kterého se skóre v rámci PROPER identifikovali podle identifikace od Microsoftu, D&B a dalších oborových standardů | 
| Plošný | Zeměpisná oblast umístění | 
| Pobočka | Dceřiná společnost zákazníka, u kterého se má skóre na Proper | 
| Sales Territory (Prodejní oblast) | Prodejní teritorium zákazníka, u kterého se provádí hodnocení Proper | 
| City (Město) | Zeměpisná poloha města | 
| State | Zeměpisné umístění stavu | 
| PSČ | Poštovní směrovací číslo organizace | 
| Country (Země) | Zeměpisná poloha země | 
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
| Cluster Microsoft 365 | Identifikuje PROPER zákazníka k nákupu Microsoft 365. Zaměřte se nyní na cíl a vyhodnoťte clustery, protože budou mít vyšší výnos. Informujte se o nurture a informujte zákazníky jenom v případě, že máte stále dostatek kapacity i po jejím zaměření a hodnocení zákazníků. | 
| Licenční program | Identifikuje typ licenčního programu pro obnovení. | 
| ID smlouvy | Identifikátor smlouvy | 
| Koncové datum smlouvy | Koncové datum smlouvy | 
| Typ vypršení platnosti | Typ vypršení platnosti | 
| Vypršení výnosů | Tržby přidružené k vypršení platnosti předplatných | 
| Má EA | Určuje, jestli je obnovení předplatného EA nebo EA. | 
| Má otevřené | Určuje, jestli je obnovování smlouva otevřené nebo otevřené hodnoty. | 
| Zákazník Azure přeprodat | Určuje, jestli zákazník zobrazuje přeprodat PROPER pro Azure. | 
| Zákazník Microsoft 365 přeprodat | Určuje, jestli zákazník zobrazuje přeprodat PROPER pro Microsoft 365. | 
| RevSumDivisionName | Identifikuje produkt, který je až pro obnovení. | 

## <a name="next-steps"></a>Další kroky

Další informace najdete v tématu [stažení sestav](pci-download-reports.md).
