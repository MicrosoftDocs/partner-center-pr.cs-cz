---
title: Definice dat Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dokument poskytuje seznam různých sestav a definice dat jednotlivých sestav, které je možné stáhnout ze stránky sestavy stažení přehledů.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/15/2020
ms.locfileid: "97502125"
---
# <a name="export--data-definitions"></a>Export – definice dat 

 **Příslušné role** 

- Prohlížeč sestav 
- Prohlížeč sestav Executive 

## <a name="introduction"></a>Úvod 

Centrum pro stažení sestav na řídicím panelu Insights umožňuje exportovat nezpracované sady dat.  

Různé sestavy, které lze stáhnout spolu s definicí dat, jsou uvedeny níže: 

**Partnerský profil**: definice dat různých polí v sestavě profilu: 


| **Název sloupce** | **Popis dat** |
|---------|:---------|
|MPNId|ID Microsoft Partner Network|
|PartnerName|Název partnera |
|PGA_MPNId|ID MPN pro globální účet partnera|
|PGA_PartnerName|Název globálního účtu partnera|
|City (Město)|Město, kde se nachází partner |
|Země|Umístění země partnera |
|HierarchyLevel|Indikuje, jestli se jedná o globální ID MPN nebo ID MPN.|

**Podrobnosti o zákaznících**: definice dat různých polí sestavy Podrobnosti o zákaznících:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|CustomerName|Jméno zákazníka |
|CustomerTenantId|ID tenanta zákazníka |
|CustomerTpid|Hlavní nadřazený identifikátor zákazníka |
|CustomerSegment|Segment zákazníka |
|CustomerMarket|Zeměpisný trh zákazníka  |
|CustomerStatus|Stav zákazníka (aktivní/Inactive) |
|Produkt|Produkt prodávaný zákazníkem MPN. Toto je jedna z O365, D365, Enterprise mobility, Power BI Microsoft Azure.|
|SKU|   SKU produktu|
|Month (Měsíc)| Měsíc, pro který se nahlásí využití a výnosy|
|MPNId| ID Microsoft Partner Network|
|PartnerName|   Název partnera|
|PartnerLocation|   Geografické umístění partnera|
|PartnerAttributionType|    Typ přidělení partnera|
|SalesChannel|  Prodejní kanál|
|AvailableSeats|    Dostupná místa| 
|RevenueUSD|    Tržby v USD|

**Výkon prodejce**: definice dat různých polí sestav o výkonu prodejců jsou tyto:

> [!Note]
> Data o výnosech a ACR jsou k dispozici pouze uživatelům, kteří jsou správci sestav od manažera.

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|ResellerMpnid|Identifikátor Microsoft Partner Network prodejce| 
|ResellerName|Jméno prodejce|
|ResellerMarket|Prodejce země na trhu| 
|IndirectProviderMPNId|Nepřímý Microsoft Partner Network identifikátor zprostředkovatele|
|IndirectProviderName|Název nepřímého zprostředkovatele|
|Month (Měsíc)|Měsíc, pro který se nahlásí využití a výnosy|
|Produkt|Název produktu|
|SubscriptionID|Identifikátor předplatného|
|AvailableSeats|Počet dostupných míst|
|AssignedSeats|Počet přiřazených stanic|
|BilledRevenueUSD|Účtované výnosy (v $)|
|CustomerName|Jméno zákazníka| 
|CustomerTPid|Hlavní nadřazený identifikátor zákazníka| 
|CustomerSegment|Segment zákazníka |
|CustomerMarket|Zeměpisný trh zákazníka |
|ResellerStatus|Stav prodejce| 

**Podrobnosti předplatných**: definice dat různých polí sestavy s podrobnostmi předplatného:

>[!Note]
>Data o výnosech a ACR jsou k dispozici pouze uživatelům, kteří jsou správci sestav od vedoucího.

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|SubscriptionId|    Identifikátor GUID předplatného|
|SubscriptionStartDate| Počáteční datum předplatného|
|SubscriptionEndDate|   Datum ukončení předplatného|
|SubscriptionState| Stav předplatného (aktivní nebo změněný)|
|Month (Měsíc)| Měsíc, pro který se nahlásí využití a výnosy|
|IsAutoRenew|   Indikuje, jestli se předplatné automaticky obnovilo (a/N).|
|CustomerName|  Název zákazníka| 
|CustomerTenantId|  GUID zákazníka|
|CustomerTpid|  Hlavní nadřazený identifikátor zákazníka| 
|CustomerSegment|   Tržní segment zákazníka| 
|CustomerMarket|    Zeměpisný trh zákazníka|
|Produkt|   Produkt prodávaný partnerem pro zákazníky| 
|SKU|   SKU produktu |
|MPNId| ID Microsoft Partner Network partnera |
|PartnerName|   Název partnera |
|PartnerLocation|   Zeměpisné umístění partnera |
|PartnerAttributionType|    Typ přidělení pro předplatné|
|SalesChannel|  Kanál prodeje (přímý/CSP atd.) |
|AvailableSeats|    Aktuální dostupné místo|
|RevenueUSD|    Tržby v USD|
|ID registrace| ID registrace předplatného|

**Využití Azure**: definice dat různých polí sestavy využití Azure:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|SubscriptionId|    Identifikátor GUID předplatného|
|SubscriptionStartDate| Datum začátku předplatného.|
|SubscriptionEndDate|   Datum, kdy předplatné skončí.|
|SubscriptionState| Aktuální stav předplatného (otevřené/uzavřené/aktivní/neposkytnutá lhůta)|
|Month (Měsíc)| Datum agregované podle měsíce |
|ServiceName|   Název služby Azure|
|MeterCategory| Název kategorie měřiče|
|UsageUnits|    Počet jednotek použitých během fakturačního cyklu |
|CustomerName|  Jméno zákazníka |
|CustomerTenantId|  ID tenanta zákazníka |
|CustomerTpid|  Hlavní ID nadřazeného zákazníka |
|CustomerSegment|   Segment zákazníka |
|CustomerMarket|    Zeměpisný trh zákazníka |
|MPNId  |ID Microsoft Partner Network zákazníka |
|PartnerName|   Název partnera |
|PartnerLocation    |Zeměpisná poloha země partnera |
|PartnerAttributionType |Typ přidělení partnera|
|SalesChannel|  Kanál prodeje (přímý/CSP nepřímo/CSP přímo atd.) |
|ACR_USD|   Využití výnosů z Azure v USD|
|ID registrace| ID registrace předplatného Azure|

**Office 365 – používání licencí**: definice dat různých polí sestavy použití sady Office 365:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|CustomerTenantId|  ID tenanta zákazníka| 
|CustomerTpid|  Hlavní ID nadřazeného zákazníka |
|Úloha úlohy|  SFB, týmy, EXO |
|Month (Měsíc)| Měsíc, pro který se nahlásí využití|
|PaidAvailableUnits|    Počet placených jednotek k dispozici|
|MonthlyActiveUsers|    Počet aktivních uživatelů za měsíc|
|CustomerName|  Jméno zákazníka|
|CustomerMarket|    Zeměpisná poloha země na trhu zákazníka |
|CustomerSegment|   Segment zákazníka |
|MPNId| ID Microsoft Partner Network|
|PartnerName|   Název partnera|
|PartnerLocation|   Geografické umístění partnera|
|PartnerAttributionType|    Typ přidělení partnera|

**Enterprise mobility – využití licencí**: definice dat různých polí sestavy používání EMS – licence:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|CustomerTenantId|  ID tenanta zákazníka| 
|CustomerTpid|  Hlavní ID nadřazeného zákazníka |
|Úloha úlohy|  Název úlohy EMS |
|Month (Měsíc)| Měsíc, pro který se nahlásí využití|
|PaidAvailableUnits|    Počet placených jednotek k dispozici|
|MonthlyActiveUsers|    Počet aktivních uživatelů za měsíc|
|CustomerName|  Jméno zákazníka|
|CustomerMarket|Zeměpisná poloha země na trhu zákazníka |
|CustomerSegment|   Segment zákazníka |
|MPNId| ID Microsoft Partner Network|
|PartnerName|   Název partnera|
|PartnerLocation|   Geografické umístění partnera|
|PartnerAttributionType|    Typ přidělení partnera|

**Dynamics 365 – použití licencí**: definice dat různých polí sestavy použití Dynamics 365 – licence:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|SubscriptionId|Identifikátor GUID předplatného|
|SubscriptionStartDate| Počáteční datum předplatného|
|SubscriptionEndDate|   Datum ukončení předplatného|
|SubscriptionStatus|    Stav předplatného |
|Month (Měsíc)| Měsíc, pro který se nahlásí využití|
|RevSumDivisionName|    Název dělení rev suma|
|RevSumCategoryName|    Název kategorie součtu rev|
|SKU|   SKU produktu |
|SKUId| ID SKU produktu |
|FreeVsPaidSKU| Označuje, zda se jedná o bezplatnou nebo placenou skladovou jednotku. |
|SalesModel|    Prodejní kanál použitý k prodeji předplatného|
|DetailedSalesModel|    Podrobný prodejní model předplatného|
|CustomerName|  Název zákazníka |
|CustomerTenantId|  Identifikátor GUID tenanta zákazníka |
|CustomerTpid|  Hlavní nadřazený identifikátor zákazníka |
|CustomerSegment|   Tržní segment zákazníka |
|CustomerMarket|    Zeměpisný trh zákazníka |
|MPNId| ID programu Microsoft Partner Network |
|PartnerName|   Název partnera |
|PartnerLocation|   Zeměpisná poloha země partnera |
|PartnerAttachType| Typ přidělení pro předplatné|
|AvailableSeats|    Aktuální dostupné místo|
|AssignedSeats| Aktuální přiřazené místo |
|ActiveSeats|   Aktuální aktivní křesla |
|DeploymentOpportunity| Aktuální příležitost nasazení|
|ActiveUsagePercent|    Aktuální procento využití v aktuálním prostředí|
 
**Power BI používání licencí**: definice dat různých polí sestavy Power BI – využití licencí:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|SubscriptionId|    Identifikátor GUID předplatného|
|SubscriptionStartDate| Počáteční datum předplatného|
|SubscriptionEndDate|   Datum ukončení předplatného|
|SubscriptionStatus|    Stav předplatného (aktivní nebo In-Active nebo v období odkladu)|
|Month (Měsíc)| Datum agregované podle měsíce |
|SKU|   SKU produktu |
|SKUId| ID SKU produktu |
|FreeVsPaidSKU| Neplacený nebo placený rozdíl SKU |
|SalesModel|    Prodejní model používaný k prodeji předplatného|
|DetailedSalesModel|    Podrobný prodejní model předplatného|
|CustomerName|  Název zákazníka |
|CustomerTenantId|  Identifikátor GUID tenanta zákazníka |
|CustomerTpid|  Hlavní nadřazený identifikátor zákazníka| 
|CustomerSegment|   Tržní segment zákazníka |
|CustomerMarket|    Zeměpisný trh zákazníka |
|MPNId| ID Microsoft Partner Network |
|PartnerName|   Název partnera |
|PartnerLocation|   Zeměpisná poloha země partnera |
|PartnerAttachType| Typ přidělení pro předplatné|
|AvailableSeats|    Aktuální dostupná místa|
|AssignedSeats| Aktuálně přiřazená místa|
|ActiveSeats|   Aktuální aktivní křesla|
|DeploymentOpportunity| Aktuální příležitost nasazení|
|ActiveUsagePercent|    Aktuální procento využití v aktuálním prostředí|

**Využití týmů – schůzky a volání**: definice dat různých polí jsou:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|CustomerTenantId|  ID tenanta zákazníka |
|CustomerTpid|  Hlavní ID nadřazeného zákazníka |
|Month (Měsíc)| Měsíc, pro který se nahlásí využití|
|Podúlohy|   Dílčí úloha, pro kterou je nahlášené využití (schůzky, hovory, telefonní systémy)|
|Počet schůzek| Počet schůzek|
|Doba trvání schůzky|  Celková doba trvání schůzky v hodinách|

**Týmy – měsíční údaje o využití**: definice dat různých polí jsou:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|CustomerTenantId|  ID tenanta zákazníka |
|CustomerTpid|  Hlavní ID nadřazeného zákazníka |
|Month (Měsíc)| Měsíc, pro který se nahlásí využití|
|Podúlohy|   Dílčí úloha, pro kterou je nahlášené využití (schůzky, hovory, telefonní systémy)|
|Uživatelé klasické pracovní plochy| Počet uživatelů, kteří používají týmy na ploše|
|Mobilní uživatele|  Počet uživatelů, kteří používají týmy na mobilních zařízeních|
|Webové uživatele| Počet uživatelů, kteří používají týmy na webu|
|AllUpParticipants| Počet různých uživatelů týmů v měsíci|

**Využití týmů – aplikace 3P**: definice dat různých polí:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|CustomerTenantId|  ID tenanta zákazníka| 
|CustomerTpid|  Hlavní ID nadřazeného zákazníka |
|Month (Měsíc)| Měsíc, pro který se nahlásí využití|
|Název aplikace 3P|   Název aplikace Teams|
|Počet uživatelů|    Počet uživatelů pro aplikaci|


**Podrobnosti o školení**: definice dat různých polí sestavy s podrobnostmi o školení:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|TrainingActivityId|    Identifikátor školení |
|TrainingTitle| Název školení |
|TrainingType|  Typ školení (certifikace/zkouška)|
|IndividualFirstName|   Křestní jméno zákazníka| 
|IndividualLastName|    Příjmení zákazníka| 
|E-mail| Osobní e-mailové ID zákazníka|
|CorpEmail| ID e-mailu pro Office zákazníka|
|TrainingCompletionDate|    Datum dokončení školení |
|Month (Měsíc)| Měsíc, pro který se data oznamují|
|IcMCP| Indikuje, jestli je uživatel ověřený Profesionálou Microsoftu.|
|MCPID| ID MCP uživatele|
|MPNId| ID Microsoft Partner Network |
|PartnerName|   Název partnera |
|PartnerCityLocation|   Zeměpisná poloha města partnera |
|PartnerCountryLocation|    Zeměpisná poloha země partnera |

**Microsoft Learn**: definice dat různých polí sestavy Microsoft Learn jsou:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|Uživatelské jméno|Jméno uživatele| 
|UserId|Identifikátor GUID uživatele |
|Procvičení|Název školení |
|TrainingType|Typ školení (/Learning cesta k modulu)|
|Produkty|Produkt, na který se vztahuje modul učení|
|Role|Příslušné role školení |
|CompletionDate|Datum dokončení školení |
|MPNId|ID Microsoft Partner Network |
|PartnerName|Název partnera |
|Země|Zeměpisná poloha země partnera |

**Souhrn kompetence a historie**: definice dat různých polí souhrnu kompetence a sestavy historie:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|CompetencyName|Název kompetence |
|CompetencyLevel|Úroveň kompetence (Gold/Silver)|
|CompetencyStatus|Aktuální stav kompetence (aktivní/neaktivní/v období odkladu)|
|CompetencyStartDate|Počáteční datum dané kompetence| 
|CompetencyEndDate|Koncové datum dané kompetence |

**Výkon kompetence**: definice dat různých polí sestavy výkonu kompetence jsou:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|CompetencyName|    Název kompetence |
|CompetencyAttainmentOptionName|    Název možnosti dosažení kompetence|
|Month (Měsíc)| Měsíc, pro který jsou hlášeny metriky|
|MetricName|    Název metriky, která se vztahuje k kompetenci|
|MetricMonthlyContribution| Měsíční příspěvek metriky|
|TTMAggregate|  Agregovaná metrika pro koncové 12 měsíců|
|AnniversaryYearAggregate|  Agregovaná metrika pro aktuální rok výročí|
|GoldThreshold| Požadavek na výkon pro splnění zlaté kompetence|
|SilverThreshold|   Požadavek na výkon pro uspokojení stříbrné kompetence|

**M365 PROPER v cloudu**: definice dat různých polí sestavy probíhající v cloudu – M365:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|ID MPN|    ID Microsoft Partner Network|
|Název partnera|  Název partnera|
|ID zákazníka|   Číslo identifikátoru zákazníka |
|DUNS číslo|   Telefonické připojení & Bradstreet číslo zákazníka, který je ve výsledku pro Proper|
|Account Name|  Název účtu |
|Doména|    Doména účtu|
|Velikost organizace|  Velikost organizace|
|Obor|  Obor  |
|Svisle|  Svislá úroveň zákazníka, který je hodnocen pro PROPER, identifikovaných Microsoftem a jinými obory standardů (D&B)|
|Oblast|  Zeměpisná oblast umístění|
|Pobočka|    Dceřiná společnost zákazníka, na kterou se skóre PROPER získává|
|Sales Territory (Prodejní oblast)|   Prodejní oblast zákazníka, se kterou se skóre PROPER vyhodnotí|
|City (Město)|  Zeměpisná poloha města |
|State| Zeměpisné umístění stavu|
|PSČ|   PSČ|
|Země|   Zeměpisná poloha země |
|Segment|   Segment trhu |
|Dílčí segment|   Dílčí segment trhu |
|Shrnutí typu SMC|  Typ SMC |
|Hlavní nespravovaný – základ COMPUTE|  Hlavní nespravované zákazníky – COMPUTE|
|Hlavní nespravovaný – základ uživatele| Hlavní nespravované zákazníky – uživatel|
|IsNonProfit|   Bez ohledu na to, jestli nezisková nebo zisková (ano/ne)|
|Povolit vzdálený pracovní cíl Exchange Online|   Zákazníci, kteří mají aktivní předplatné Exchange Online, přeprodat na M365|
|Povolit vzdálenou práci na Prem (aktuální verze) pomocí CLAS PROPER – + 10 licencí|Zákazník, který má aktuálního klienta Office nebo Win Prem (tj. verze, které jsou po EOS Products). Zákazník má 10 nebo více licencí. Zákazník, který má skóre proper. Partneři by měli cílit na převod na M365.|
|Povolit vzdálené zpracování Prem (aktuální verze) pomocí CLASch per – <10 licencí|Zákazník, který má aktuálního klienta Office nebo Win Prem (tj. verze, které jsou po EOS Products). Zákazník má méně než 10 licencí. Zákazník, který má skóre proper. Partneři by měli cílit na převod na M365.|
|Povolit vzdálené získání Prem (aktuální verze) bez CLASch per – + 10 licencí| Zákazník, který má aktuálního klienta Office nebo Win Prem (tj. verze, které jsou po EOS Products). Zákazník má 10 nebo více licencí. Zákazník nemá skóre proper. Partneři by měli cílit na převod na M365.|
|Povolit vzdálené získání Prem (aktuální verze) bez CLASch per – <10 licencí| Zákazník, který má aktuálního klienta Office nebo Win Prem (tj. verze, které jsou po EOS Products). Zákazník má méně než 10 licencí. Zákazník nemá skóre proper. Partneři by měli cílit na převod na M365.|
|Povolení vzdáleného řešení Prem (EOS) s licencemi CLAS – + 10|Zákazník, který má EOS on-Prem klienta Office nebo Win (tj. verze, které jsou starší než a včetně produktů EOS). Zákazník má 10 nebo více licencí. Zákazník má skóre proper. Partneři by měli cílit na převod na M365.|
|Povolení vzdáleného řešení Prem (EOS) s využitím CLASch PROPER – licence <10|Zákazník, který má EOS on-Prem klienta Office nebo Win (tj. verze, které jsou starší než a včetně produktů EOS). Zákazník má méně než 10 licencí. Zákazník má skóre proper. Partneři by měli cílit na převod na M365.|
|Povolit vzdálené zpracování Prem (EOS) bez dalších CLASch PROPER – + 10 licencí| Zákazník, který má aktuálního klienta Office nebo Win Prem (tj. verze, které jsou starší než a včetně EOS Products). Zákazník má 10 nebo více licencí. Zákazník nemá skóre proper. Partneři by měli cílit na převod na M365.|
|Povolit vzdálené zpracování Prem (EOS) bez CLASch PROPER – licence <10| Zákazník, který má aktuálního klienta Office nebo Win Prem (tj. verze, které jsou starší než a včetně EOS Products). Zákazník má méně než 10 licencí. Zákazník nemá skóre proper. Partneři by měli cílit na převod na M365.|
|Povolit vzdálený pracovní postup s vysokou mírou prohlídky pro M365 (ACT nyní/vyhodnotit)| Zákazník s vysokou mírou prohlídky pro M365.|
|Povolení vzdálené práce – Soutěžování (přiblížení) pomocí M365| Zákazníci s přiblížením a M365 cíli pro převod na týmy|
|Povolit vzdálenou práci – soutěžit (Lupa) bez M365|  Zákazníci s přiblížením, cíli pro převod na týmy|
|Snižte náklady a spravujte – M365 E3 cílené na M365 E5| Stávající zákazník s M365 E3, cíl pro M365 E5|
|Snižte náklady a spravujte – M365 a BS – zákazníky cílené na M365 BP|    Stávající zákazníci M365 BB a BS, cílí na tyto M365 BP|
|Transformace produktivity organizace – PROPER Surface|    Zákazník zobrazuje PROPER pro plochu.|
|M365Cluster|Identifikuje PROPER zákazníka k nákupu M365.  Clustery teď fungují a vyhodnocení by se mělo zaměřit, protože budou mít vyšší výnos.  Nurture a pedagogy by se měly zaměřit jenom v případě, že stále existuje kapacita, po jejímž uplynutí se zaměřuje a vyhodnotí zákazníky.|
|M365Fit|   Interní a externí datové body, které definují firmographics. Pro účely bodování se používá model podobného typu, který umožňuje porovnat zákazníky a zjistit, jestli jsou potenciálně vyhovující Microsoft Cloud produktů. Vyhodnocování podle skóre se aktualizuje čtvrtletně.|
|M365Intent|    Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení, aby bylo možné definovat clustery. Bodování záměru se aktualizuje měsíčně.|
|SurfaceCluster|    Tím se identifikují prohlédnutí zákazníka, které připadá na plochu tím, že se do clusteru konsolidují doporučení k přizpůsobení a záměrům.  Clustery teď fungují a vyhodnocení by se mělo zaměřit, protože budou mít vyšší výnos.  Nurture a pedagogy by se měly zaměřit jenom v případě, že stále existuje kapacita, po jejímž uplynutí se zaměřuje a vyhodnotí zákazníky.|
|SurfaceFit|    Interní a externí datové body, které definují firmographics. Pro účely bodování se používá model podobného typu, který umožňuje porovnat zákazníky a zjistit, jestli jsou potenciálně vyhovující Microsoft Cloud produktů. Vyhodnocování podle skóre se aktualizuje čtvrtletně.|
|SurfaceIntent| Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení, aby bylo možné definovat clustery. Bodování záměru se aktualizuje měsíčně.|
|O365Cluster|   To identifikuje PROPER zákazníka k nákupu O365.  Clustery teď fungují a vyhodnocení by se mělo zaměřit, protože budou mít vyšší výnos.  Nurture a pedagogy by se měly zaměřit jenom v případě, že stále existuje kapacita, po jejímž uplynutí se zaměřuje a vyhodnotí zákazníky.|
|O365Fit|   Interní a externí datové body, které definují firmographics. Pro účely bodování se používá model podobného typu, který umožňuje porovnat zákazníky a zjistit, jestli jsou potenciálně vyhovující Microsoft Cloud produktů. Vyhodnocování podle skóre se aktualizuje čtvrtletně.|
|O365Intent|    Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení, aby bylo možné definovat clustery. Bodování záměru se aktualizuje měsíčně.|
|M365UpsellCustomer|    Určuje, jestli zákazník zobrazuje přeprodat PROPER pro M365.|
|Má Google|    Tento příznak označuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnictví produktů Google.|
|Má AWS|   Tento příznak identifikuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnící produkty v AWS.|
|Má EA|    To označuje, jestli se obnovení provádí v rámci smlouvy Enterprise (EA) nebo předplatného EA.|
|Má otevřené|  Tato hodnota označuje, zda je prodloužení platnosti otevřené nebo otevřené.|

**D365 PROPER v cloudu**: definice dat různých polí sestavy probíhající v cloudu – D365:

| **Název sloupce** | **Popis dat** |
|---------|:---------|
|ID MPN|    ID Microsoft Partner Network|
|Název partnera|  Název partnera|
|ID zákazníka|   Číslo identifikátoru zákazníka |
|DUNS číslo|   Telefonické připojení & Bradstreet číslo zákazníka, který je ve výsledku pro Proper|
|Account Name|  Název účtu |
|Doména|    Doména účtu|
|Velikost organizace|  Velikost organizace|
|Obor|  Obor  |
|Svisle|  Svislá úroveň zákazníka, který je hodnocen pro PROPER, identifikovaných Microsoftem a jinými obory standardů (D&B)
|Oblast|  Zeměpisná oblast umístění|
|Pobočka|    Dceřiná společnost zákazníka, na kterou se skóre PROPER získává|
|Sales Territory (Prodejní oblast)|   Sales Territory (Prodejní oblast)|
|City (Město)|  Zeměpisná poloha města |
|State| Zeměpisné umístění stavu|
|PSČ|   PSČ|
|Země|   Zeměpisná poloha země |
|Segment|   Segment trhu |
|Dílčí segment|   Dílčí segment trhu |
|Shrnutí typu SMC|  Kategorizace zákazníka: hlavní nespravované uživatelské základy jsou zákazníky, kteří mají více než 300 zaměstnanců, hlavní nespravovaný výpočetní základ pro zákazníky s 25 000 možnostmi na Azure 3 roky – středně velké firmy jsou zákazníci s 25 zaměstnanci nebo vyšší, malé firmy jsou zákazníky s méně než 25 zaměstnanci.|
|Hlavní nespravovaný – základ COMPUTE   |Hlavní nespravované zákazníky – COMPUTE|
|Hlavní nespravovaný – základ uživatele| Hlavní nespravované zákazníky – uživatelé|
|IsNonProfit|   Bez ohledu na to, jestli nezisková nebo zisková (ano/ne)|
|Aktivovat digitální prodej – M365-velikost sedadel >= 25 míst (model SalesProch per)|   Zákazník bez D365. Velikost sedadla: 25 +. Partneři by měli cílit na vzájemný prodej D365 Salespro.|
|Aktivace D365ch per pro digitální prodej – SalesPro (ACT Now/Evaluate) |Vysoce propers zákazníkům bez D365.  Partneři by měli cílit na D365 SalesPro.|
|Správa finančního rizika & podvodů – Dynamics on-Prem instalace modelu základní-Navision (BC – model PROPER)|Stávající zákazník s OnPrem Navision.  Partner by měl cílit na D365 BC.|
|Správa finančních rizik & podvodů – Prem instalace aplikace pro základní-AX (F&O properech)    |Stávající zákazník s OnPrem AX.  Partner by měl cílit na D365 F&O|
|Správa finančních rizik & podvodů – Prem instalace na základní-Skvělé Plains (model PROPER BC)|  Stávající zákazník s OnPrem Skvělé Plains.  Partner by měl cílit na D365 BC.|
|Správa finančních rizik & podvodů – Dynamics on-Prem instalace základní-Šalamounovy (BC) – model Proper|Stávající zákazník s OnPrem Solomonem.  Partner by měl cílit na D365 BC.|
|Správa finančních rizik & podvodů – Dynamics on-Prem instalace základních – dalších (BC – model PROPER) |Stávající zákazník s dalšími OnPrem řešeními, která nejsou uvedená výše.  Partner by měl cílit na D365 BC.|
|Sestavování agilních obchodních procesů – Dynamics on-Prem instalace Base-AX/GP/SL/NAV/Other (model D365 PROPER)|   Sestavování agilních obchodních procesů – Dynamics on-Prem instalace Base-AX/GP/SL/NAV/Other (model D365 PROPER)|
|Sestavování agilních obchodních procesů – dynamika konkurenčních bází – Mendix/subsystému/Salesforce (D365 model PROPER)| Sestavování agilních obchodních procesů – dynamika konkurenčních bází – Mendix/subsystému/Salesforce (D365 model PROPER)|
|Sestavování agilních obchodních procesů – D365 F&O instalační bázi |Stávající zákazníci D365 F&O.  Partner pro cílení Power Apps.|
|Sestavování agilních obchodních procesů – D365 BC – základ instalace| Stávající zákazníci D365 BC. Partner pro cílení Power Apps.|
|Vytváření agilních obchodních procesů – základ instalace D365 CE| Stávající zákazníci D365 CE. Partner pro cílení Power Apps.|
|Sestavení odolného dodavatelského řetězce – výher a aktivace prvního D365 úlohy jako D365 dodavatelských řetězců s zákazníky, kteří nejsou Oracle/SAP ERP|  Cílové zákazníky pro dodavatelský řetězec D365|
|Sestavte odolný dodavatelský řetězec – meziprodejní D365 dodavatelský řetězec a/nebo maloobchod/obchod s existujícími zákazníky D365 CE. |Stávající zákazníci D365 CE cílí na D365 dodavatelských řetězců mezi prodejy|
|Sestavte odolný dodavatelský řetězec – vzájemný prodej D365 sup. Řetězení a/nebo maloobchod/obchod s D365 CE a (Oracle nebo SAP)| Stávající zákazníci D365 CE s Oracle nebo SAP pro cílení na dodavatelský řetězec D365|
|D365BCCluster| Tím se identifikují PROPER zákazníka, která si koupí D365 Business Central.  Zákazníci, kteří zobrazují PROPER pro BC, budou mít střední a malé kategorie.  Clustery teď fungují a vyhodnocení by se mělo zaměřit, protože budou mít vyšší výnos.  Nurture a pedagogy by se měly zaměřit jenom v případě, že stále existuje kapacita, po jejímž uplynutí se zaměřuje a vyhodnotí zákazníky.|
|D365BCFit| Interní a externí datové body, které definují firmographics. Pro účely bodování se používá model podobného typu, který umožňuje porovnat zákazníky a zjistit, jestli jsou potenciálně vyhovující Microsoft Cloud produktů. Vyhodnocování podle skóre se aktualizuje čtvrtletně.|
|D365BCIntent|  Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení, aby bylo možné definovat clustery. Bodování záměru se aktualizuje měsíčně.|
|D365FOCluster| Tím se identifikují PROPER zákazníka, aby si koupili D365 finance a operace.  Zákazníci, kteří zobrazují PROPER pro F&O, budou v hlavních nespravovaných kategoriích. Clustery teď fungují a vyhodnocení by se mělo zaměřit, protože budou mít vyšší výnos.  Nurture a pedagogy by se měly zaměřit jenom v případě, že stále existuje kapacita, po jejímž uplynutí se zaměřuje a vyhodnotí zákazníky.|
|D365FOFit| Interní a externí datové body, které definují firmographics. Pro účely bodování se používá model podobného typu, který umožňuje porovnat zákazníky a zjistit, jestli jsou potenciálně vyhovující Microsoft Cloud produktů. Vyhodnocování podle skóre se aktualizuje čtvrtletně.|
|D365FOIntent|  Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení, aby bylo možné definovat clustery. Bodování záměru se aktualizuje měsíčně.|
|D365CECluster| Tím se identifikují PROPER zákazníka, aby si koupili D365 zákaznickou zapojení.  Zákazníci, kteří zobrazují PROPER pro CE, budou ve středních a malých kategoriích.  Clustery teď fungují a vyhodnocení by se mělo zaměřit, protože budou mít vyšší výnos.  Nurture a pedagogy by se měly zaměřit jenom v případě, že stále existuje kapacita, po jejímž uplynutí se zaměřuje a vyhodnotí zákazníky.|
|D365CEFit| Přizpůsobit pro D365 CE|
|D365CEIntent|  Záměr pro D365 CE|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  Určuje, jestli má zákazník otevřené obnovení pro Dynamics on-Prem AX nebo CRM.|
|M365UpsellCustomer|    Určuje, jestli zákazník zobrazuje přeprodat PROPER pro M365.|
|Má Google|    Tento příznak označuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnictví produktů Google.|
|Má AWS|   Tento příznak identifikuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnící produkty v AWS.|
|Má EA |To označuje, jestli se obnovení provádí v rámci smlouvy Enterprise (EA) nebo předplatného EA.|
|Má otevřené|  Tato hodnota označuje, zda je prodloužení platnosti otevřené nebo otevřené.|

**Cloud Ascent-Azure PROPER**: definice dat různých polí sestavy cloudových Ascent-Azurech PROPER:

|**Název sloupce** |**Popis dat** |
|---------|:---------|
|ID MPN|    ID Microsoft Partner Network|
|Název partnera|  Název partnera|
|ID zákazníka|   Číslo identifikátoru zákazníka |
|DUNS číslo|   Telefonické připojení & Bradstreet číslo zákazníka, který je ve výsledku pro Proper|
|Account Name|  Název účtu |
|Doména|    Doména účtu|
|Velikost organizace|  Velikost organizace|
|Obor|  Obor  |
|Svisle|  Svislá úroveň zákazníka, který je hodnocen pro PROPER, identifikovaných Microsoftem a jinými obory standardů (D&B)|
|Oblast|  Zeměpisná oblast umístění|
|Pobočka|    Dceřiná společnost zákazníka, na kterou se skóre PROPER získává|
|Sales Territory (Prodejní oblast)|   Sales Territory (Prodejní oblast)|
|City (Město)|  Zeměpisná poloha města |
|State| Zeměpisné umístění stavu|
|PSČ|   PSČ|
|Země|   Zeměpisná poloha země |
|Segment|   Segment trhu |
|Dílčí segment|   Dílčí segment trhu |
|Shrnutí typu SMC|  Typ SMC |
|Hlavní nespravovaný – základ COMPUTE|  Hlavní nespravované zákazníky – COMPUTE|
|Hlavní nespravovaný – základ uživatele| Hlavní nespravované zákazníky – uživatelé|
|IsNonProfit|   Bez ohledu na to, jestli nezisková nebo zisková (ano/ne)|
|Migrace – EOS Win Server – EOS Windows Server IB s CLAS – 5 a licence|   Zákazník, který má EOS na Prem Win serveru (tj. verze, které jsou starší než a včetně produktů EOS). Zákazník má 5 nebo více licencí. Zákazník, který má skóre proper.  Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – EOS Win Server – EOS Windows Server IB s CLAS-<5 licencí|   Zákazník, který má EOS (end Service) na Prem Win Server (tj. verze, které jsou starší než a včetně produktů EOS). Zákazník má méně než 5 licencí. Zákazník, který má skóre proper.  Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – EOS Win Server – EOS Windows Server IB bez CLAS PROPER – 5 a licence |Zákazník, který má EOS na Prem Win serveru (tj. verze, které jsou starší než a včetně produktů EOS). Zákazník má více než 5 licencí. Zákazník nemá skóre proper. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – EOS Win Server – EOS Windows Server IB bez CLAS PROPER – licence <5|    Zákazník, který má EOS na Prem Win serveru (tj. verze, které jsou starší než a včetně produktů EOS). Má méně než 5 licencí. Zákazník nemá skóre proper. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – EOS SQL-EOS SQL Server IB s CLASmi Promi – 5 a licence|  Zákazník, který má EOS on-Prem SQL Server (tj. verze, které jsou starší než a včetně produktů EOS). Zákazník má 5 licencí. Zákazník má skóre proper.  Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – EOS SQL-EOS SQL Server IB s CLAS – <5 licencí|  Zákazník, který má EOS on-Prem SQL Server (tj. verze, které jsou starší než a včetně produktů EOS). Má méně než 5 licencí. Zákazník, který má skóre proper. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – EOS SQL-EOS SQL Server IB bez CLAS PROPER – 5 a licence|   Zákazník, který má EOS on-Prem SQL Server (tj. verze, které jsou starší než a včetně produktů EOS). Zákazník má 5 nebo více licencí. Zákazník nemá skóre proper. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – EOS SQL-EOS SQL Server IB bez CLAS PROPER – <5 licencí|   Zákazník, který má EOS on-Prem SQL Server (tj. verze, které jsou starší než a včetně produktů EOS). Zákazník má méně než 5 licencí. Zákazník nemá skóre proper. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – migrace Prem Win serveru – aktuální Windows Server IB s CLAS PROPER-5 + licence|   Zákazník, který má aktuální Prem Win Server (tj. verze, které jsou po EOS produktech). Zákazník má 5 licencí. Zákazník má skóre proper. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – migrace Prem Win serveru – aktuální Windows Server IB s CLAS PROPER-<5 licencí|   Zákazník, který má aktuální Prem Win Server (tj. verze, které jsou po EOS produktech). Zákazník má méně než 5 licencí. Zákazník má skóre PROPER pro Azure. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – migrace Prem Win serveru – aktuální Windows Server IB bez CLAS PROPER – 5 a licence|    Zákazník, který má aktuální Prem Win Server (tj. verze, které jsou po EOS produktech). Zákazník má 5 licencí. Zákazník nemá skóre proper. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – migrace Prem Win serveru – aktuální Windows Server IB bez CLAS PROPER-<5 licencí |Zákazník, který má aktuální Prem Win Server (tj. verze, které jsou po EOS produktech). Zákazník má méně než 5 licencí. Zákazník nemá skóre proper. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – migrace na virtuální počítače Azure SQL nebo SQL – aktuální SQL Server IB s CLASmi PROPER – 5 a licence|  Zákazník, který má aktuální Prem SQL Server (tj. verze, které jsou po EOS produktech). Zákazník má 5 licencí. Zákazník má skóre proper. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – migrace na virtuální počítače Azure SQL nebo SQL – aktuální SQL Server v IB s použitím CLASch PROPER – <5 licencí|  Zákazník, který má aktuální Prem SQL Server (tj. verze, které jsou po EOS produktech). Zákazník má méně než 5 licencí. Zákazník má skóre proper. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – migrace na virtuální počítače Azure SQL nebo SQL – aktuální SQL Server IB bez CLASch PROPER – 5 a licence|   Zákazník, který má aktuální Prem SQL Server (tj. verze, které jsou po EOS produktech). Zákazník má 5 licencí. Zákazník nemá skóre proper. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – migrace na virtuální počítače Azure SQL nebo SQL – aktuální SQL Server IB bez CLASch PROPER – <5 licencí|   Zákazník, který má aktuální Prem SQL Server (tj. verze, které jsou po EOS produktech). Zákazník má méně než 5 licencí. Zákazník nemá skóre proper. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – OSS – migrace na OSS DB| Stávající zákazník s některým z následujících konkurenčních produktů: PostgreSQL, MySQL, MariaDB. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – OSS-Linux v Azure |Stávající zákazník s produktem: Linux. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – SAP-SAP v Azure|  Stávající zákazník s produktem: SAP. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – WVD – RDS IB |Identifikuje zákazníky s aktivní službou Vzdálená plocha systému Windows. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – WVD – moderní práce v různých prodejích do Azure/WVD|   Identifikuje zákazníky s M365 a nemá Azure. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – VMware IB|   Stávající zákazník s produktem: VMware. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Migrace – Citrix IB|   Stávající zákazník s produktem: systémy Citrix. Partneři by měli cílit na tyto zákazníky na migraci do Azure.|
|Inovace – analýza – Power BI IB a vysoké PROPER Azure|   Zákazníci s předplatným a aktivním Power BI, včetně: Power BI-Standalone pro, Power BI – sady pro Azure, sady Power BI sady Office, Power BI sady – M365|
|Enable-DevOps with GitHub-VisualStudio/MSDN IB|    Identifikováni zákazníci s aktivní sadou Visual studia|
|Verze serveru Win Standard|   Zobrazuje verzi Windows serveru standard pro nákupy podle zákazníka.|
|Standardní licence systému Win Server|   Zobrazuje se typ licence pro nákupy Windows serveru Standard zákazníkem.|
|Verze datového centra serveru Win|    Zobrazuje verzi Windows Data Center – nákupy podle zákazníka|
|Licence datového centra serveru Win| Zobrazuje se typ licence pro nákup datového centra Windows podle zákazníka.|
|AzureFit|  Interní a externí datové body, které definují firmographics. Pro účely bodování se používá model podobného typu, který umožňuje porovnat zákazníky a zjistit, jestli jsou potenciálně vyhovující Microsoft Cloud produktů. Vyhodnocování podle skóre se aktualizuje čtvrtletně.|
|AzureIntent|   Signály týkající se sociálních médií a definování záměrů online zákazníka. Bodování záměru je překrytí na základě přizpůsobení, aby bylo možné definovat clustery. Bodování záměru se aktualizuje měsíčně.|
|AzureCluster|  Tím se identifikují prohlédnutí zákazníka, které vám umožní koupit Azure tím, že se do clusteru konsolidují doporučení k přizpůsobení a záměrům.  Clustery teď fungují a vyhodnocení by se mělo zaměřit, protože budou mít vyšší výnos.  Nurture a pedagogy by se měly zaměřit jenom v případě, že stále existuje kapacita, po jejímž uplynutí se zaměřuje a vyhodnotí zákazníky.|
|WindowsServerDataCenter_HasOpenRenewal|    Označuje, jestli má zákazník otevřené obnovení pro datové centrum Windows serveru.|
|WindowsServerStandard_HasOpenRenewal|  Určuje, jestli má zákazník otevřené obnovení pro Windows Server Standard.|
|AzureUpsellCustomer|   Určuje, jestli zákazník zobrazuje přeprodat PROPER pro Azure.|
|Má Google|    Tento příznak označuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnictví produktů Google.|
|Má AWS|   Tento příznak identifikuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnící produkty v AWS.|
|Má EA |To označuje, jestli se obnovení provádí v rámci smlouvy Enterprise (EA) nebo předplatného EA.|
|Má otevřené|  Tato hodnota označuje, zda je prodloužení platnosti otevřené nebo otevřené.|

**Obnovení PROPER v cloudu Ascent-Agreement**: definice dat různých polí sestavy probíhající se obnovením smluv v cloudu:

|**Název sloupce** |**Popis dat** |
|---------|:---------|
|ID MPN|    ID Microsoft Partner Network|
|Název partnera|  Název partnera|
|ID zákazníka|   Číslo identifikátoru zákazníka |
|DUNS číslo|   Telefonické připojení & Bradstreet číslo zákazníka, který je ve výsledku pro Proper|
|Account Name|  Název účtu |
|Doména|    Doména účtu|
|Velikost organizace|  Velikost organizace|
|Obor|  Obor  |
|Svisle|  Svislá úroveň zákazníka, který je hodnocen pro PROPER, identifikovaných Microsoftem a jinými obory standardů (D&B)|
|Oblast|  Zeměpisná oblast umístění|
|Pobočka|    Dceřiná společnost zákazníka, na kterou se skóre PROPER získává|
|Sales Territory (Prodejní oblast)|   Sales Territory (Prodejní oblast)|
|City (Město)|  Zeměpisná poloha města |
|State| Zeměpisné umístění stavu|
|PSČ|   PSČ|
|Země|   Zeměpisná poloha země |
|Segment|   Segment trhu |
|Dílčí segment|   Dílčí segment trhu |
|Shrnutí typu SMC|  Typ SMC |
|Hlavní nespravovaný – základ COMPUTE|  Hlavní nespravované zákazníky – COMPUTE|
|Hlavní nespravovaný – základ uživatele| Hlavní nespravované zákazníky – uživatelé|
|IsNonProfit|Bez ohledu na to, jestli nezisková nebo zisková (ano/ne)|
|Má Google|Tento příznak identifikuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnící produkty v AWS.|
|Má AWS|Tento příznak identifikuje, jestli zákazník zobrazuje signály konkurenčních signálů pro vlastnící produkty v AWS.|
|Cluster Azure|Tím se identifikují PROPER zákazníka k nákupu Azure.  Clustery teď fungují a vyhodnocení by se mělo zaměřit, protože budou mít vyšší výnos.  Nurture a pedagogy by se měly zaměřit jenom v případě, že stále existuje kapacita, po jejímž uplynutí se zaměřuje a vyhodnotí zákazníky.|
|D365 F&v clusteru|  Tím se identifikují PROPER zákazníka, aby si koupili D365 finance a operace.  Zákazníci, kteří zobrazují PROPER pro F&O, budou v hlavních nespravovaných kategoriích.  Clustery teď fungují a vyhodnocení by se mělo zaměřit, protože budou mít vyšší výnos.  Nurture a pedagogy by se měly zaměřit jenom v případě, že stále existuje kapacita, po jejímž uplynutí se zaměřuje a vyhodnotí zákazníky.|
|Cluster D365 CE|   Tím se identifikují PROPER zákazníka, aby si koupili D365 zákaznickou zapojení.  Zákazníci, kteří zobrazují PROPER pro CE, budou ve středních a malých kategoriích.  Clustery teď fungují a vyhodnocení by se mělo zaměřit, protože budou mít vyšší výnos.  Nurture a pedagogy by se měly zaměřit jenom v případě, že stále existuje kapacita, po jejímž uplynutí se zaměřuje a vyhodnotí zákazníky.|
|Cluster D365 BC|   Tím se identifikují PROPER zákazníka, která si koupí D365 Business Central.  Zákazníci, kteří zobrazují PROPER pro BC, budou mít střední a malé kategorie.  Clustery teď fungují a vyhodnocení by se mělo zaměřit, protože budou mít vyšší výnos.  Nurture a pedagogy by se měly zaměřit jenom v případě, že stále existuje kapacita, po jejímž uplynutí se zaměřuje a vyhodnotí zákazníky.|
|Cluster M365|  Tím se identifikují proM365y zákazníka, které slouží k nákupu.  Clustery teď fungují a vyhodnocení by se mělo zaměřit, protože budou mít vyšší výnos.  Nurture a pedagogy by se měly zaměřit jenom v případě, že stále existuje kapacita, po jejímž uplynutí se zaměřuje a vyhodnotí zákazníky.|
|Licenční program|   Identifikuje typ licenčního programu pro obnovení.|
|ID smlouvy|  Identifikátor smlouvy|
|Koncové datum smlouvy|    Koncové datum smlouvy |
|Typ vypršení platnosti|   Typ vypršení platnosti|
|Vypršení výnosů|  Tržby přidružené k vypršení platnosti předplatných|
|Má EA|    To označuje, jestli se obnovení provádí v rámci smlouvy Enterprise (EA) nebo předplatného EA.|
|Má otevřené|  Tato hodnota označuje, zda je prodloužení platnosti otevřené nebo otevřené.|
|Zákazník Azure přeprodat| Určuje, jestli zákazník zobrazuje přeprodat PROPER pro Azure.|
|Zákazník M365 přeprodat|  Určuje, jestli zákazník zobrazuje přeprodat PROPER pro M365.|
|RevSumDivisionName|    Označuje produkt, který je až pro obnovení.|

## <a name="next-steps"></a>Další kroky

Informace o sestavách najdete v tématu [stažení sestav](pci-download-reports.md).
