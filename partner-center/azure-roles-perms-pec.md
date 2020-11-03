---
title: Role, oprávnění pro realizované kredity partnerů
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si o rolích a oprávněních pro partnery, kteří budou moci získat kredity získané prostřednictvím partnerů. Ty se liší od rolí pro práci v partnerském centru.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f48774cb830ceb575a84177efb57431afdcb9b25
ms.sourcegitcommit: 5fc28f6f81eaebb84e1faa71848afb504e181f37
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/11/2020
ms.locfileid: "92527236"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>Role a oprávnění, která mají nárok na získání realizovaného kreditu partnerů

Následující role se mapují na úrovně oprávnění, které určují, jestli má partner nárok na získané kredity partnerů.

>[!Important]
>Tyto role a oprávnění nejsou stejné jako role a oprávnění, která uživatel potřebuje k práci v partnerském centru.

|**Role**   |**Popis**   |**Způsobilý pro PEC**   |
|-----------------|:------------------|:--------------|
|Vlastník  |Všechno můžete spravovat, včetně přístupu k prostředkům.|Ano|
|Přispěvatel |Vše můžete spravovat kromě udělení přístupu k prostředkům.|Ano|
|Čtenář|Můžete zobrazit vše, ale ne provádět žádné změny.|Ne|
|ACRDelete|Odstranit ACR|Ano|
|ACRImageSigner|podpis ACR image|Ano|
|ACRPull|ACR pull|Ano|
|AcrPush|nabízení ACR|Ano|
|AcrQuarantineReader|čtečka dat karantény ACR|Ne|
|AcrQuarantineWriter| zapisovač dat karantény ACR|Ano|
|Přispěvatel API Management služby|Může spravovat službu a rozhraní API.|Ano|
|Role operátora služby API Management|Může spravovat službu, ale ne rozhraní API.|Ano|
|Role čtecího modulu služby API Management|Přístup ke službě a rozhraním API jen pro čtení|Ne|
|Přispěvatel Application Insights komponent|Spravuje Application Insights komponenty.|Ano|
|Application Insights Snapshot Debugger|Poskytuje uživateli oprávnění k zobrazení a stažení snímků ladění shromážděných pomocí Snapshot Debugger Application Insights. Všimněte si, že tato oprávnění nejsou zahrnutá v rolích vlastník nebo Přispěvatel.|Ano|
Operátor úlohy služby Automation | Vytvářejte a spravujte úlohy pomocí runbooků Automation. | Ano | 
Operátor služby Automation | Operátory automatizace můžou spouštět, zastavovat, pozastavovat a obnovovat úlohy. | Ano | 
Operátor Runbooku služby Automation | Číst vlastnosti Runbooku – abyste mohli vytvářet úlohy Runbooku. | Ano | 
Přispěvatel avere | Může vytvořit a spravovat cluster avere vFXT. | Ano | 
Avere – operátor | Používá cluster avere vFXT ke správě clusteru. | Ano | 
Vlastník dat Event Hubs Azure | Umožňuje úplný přístup k prostředkům Azure Event Hubs. | Ano | 
Přijímač dat Event Hubs Azure | Umožňuje získat přístup k prostředkům Azure Event Hubs. | Ano | 
Odesilatel dat Event Hubs Azure | Povoluje odesílání přístup k prostředkům Azure Event Hubs. | Ano | 
Role Správce clusteru služby Azure Kubernetes | Vypíše akci přihlašovacích údajů správce clusteru. | Ano | 
Role uživatele clusteru služby Azure Kubernetes | Vypíše akci přihlašovacích údajů uživatele clusteru. | Ano | 
Čtečka dat Azure Maps (Preview) | Udělí přístup ke čtení dat souvisejících s mapou z účtu Azure Maps. | Ne | 
Azure Service Bus vlastník dat | Umožňuje úplný přístup k Azure Service Bus prostředkům. | Ano | 
Azure Service Bus přijímač dat | Umožňuje získat přístup k prostředkům Azure Service Bus. | Ano | 
Azure Service Bus odesílatel dat | Umožňuje odeslat přístup k prostředkům Azure Service Bus. | Ano | 
Vlastník registrace Azure Stack | Umožňuje spravovat Azure Stack registrace. | Ano | 
Přispěvatel zálohování | Umožňuje správu služby zálohování, ale nemůže vytvářet trezory a udělovat přístup jiným uživatelům. | Ano | 
Operátor zálohování | Umožňuje správu zálohovacích služeb s výjimkou odebrání zálohování, vytváření trezoru a poskytování přístupu jiným uživatelům. | Ano | 
Čtečka zálohování | Může zobrazovat služby zálohování, ale nemůže provádět změny. | Ne | 
Čtenář fakturace | Povolí přístup pro čtení k fakturačním údajům. | Ne | 
Přispěvatel BizTalk | Umožňuje spravovat BizTalk Services, ale ne přístup k nim. | Ano | 
Přístup ke členskému uzlu blockchain (Preview) | Umožňuje přístup k blockchain členským uzlům. | Ano | 
Přispěvatel podrobného plánu | Může spravovat definice podrobného plánu, ale nepřiřazovat je. | Ano | 
Operátor podrobného plánu | Může přiřadit existující publikované modrotisky, ale nemůže vytvářet nové plány. Poznámka: Tato akce funguje pouze v případě, že je přiřazení provedeno pomocí uživatelem přiřazené spravované identity. | Ano | 
Přispěvatel koncového bodu CDN | Může spravovat koncové body CDN, ale nemůže udělit přístup jiným uživatelům. | Ano | 
Čtečka koncového bodu CDN | Může zobrazovat koncové body CDN, ale nemůže provádět změny. | Ne | 
Přispěvatel profilu CDN | Může spravovat profily CDN a jejich koncové body, ale nemůže udělit přístup jiným uživatelům. | Ano | 
Čtečka profilů CDN | Může zobrazit profily CDN a jejich koncové body, ale nemůže provádět změny. | Ne | 
Přispěvatel klasických sítí | Umožňuje správu klasických sítí, ale ne přístup k nim. | Ano | 
Přispěvatel klasických účtů úložiště | Umožňuje správu klasických účtů úložiště, ale ne přístup k nim. | Ano | 
Role služby operátora klíče klasického účtu úložiště | Operátoři klíčů pro klasický účet úložiště můžou vypisovat a znovu generovat klíče na klasických účtech úložiště. | Ano | 
Přispěvatel klasických virtuálních počítačů | Umožňuje správu klasických virtuálních počítačů, ale ne přístup k nim ani k virtuální síti nebo účtu úložiště, ke kterým se připojuje. | Ano | 
Přispěvatel Cognitive Services | Umožňuje vytvářet, číst, aktualizovat, odstraňovat a spravovat klíče Cognitive Services. | Ano | 
Čtečka dat Cognitive Services (Preview) | Umožňuje číst Cognitive Services data. | Ne | 
Cognitive Services uživatel | Umožňuje číst a zobrazit seznam klíčů Cognitive Services. | Ne | 
Role čtečky účtu Cosmos DB | Může číst data Azure Cosmos DB účtu. Správa účtů Azure Cosmos DB najdete v tématu Přispěvatel účtu DocumentDB. | Ne | 
Operátor Cosmos DB | Umožňuje správu účtů Azure Cosmos DB, ale ne přístup k datům v nich. Zabraňuje přístup k klíčům účtu a připojovacím řetězcům. | Ano | 
CosmosBackupOperator | Může odeslat žádost o obnovení pro Cosmos DB databázi nebo kontejner pro účet. | Ano | 
Přispěvatel Cost Management | Umožňuje zobrazit náklady a spravovat konfiguraci nákladů (např. rozpočty, exporty). | Ano | 
Čtecí modul Cost Management | Může zobrazit data a konfiguraci nákladů (např. rozpočty, exporty). | Ne | 
Přispěvatel Data Box | Umožňuje spravovat všechno, co služba Data Box, s výjimkou poskytnutí přístupu jiným uživatelům. | Ano | 
Čtecí modul Data Box | Umožňuje správu Data Box služby s výjimkou vytváření pořadí nebo úprav podrobností objednávky a udělení přístupu jiným uživatelům. | Ne | 
Přispěvatel Data Factory | Vytváření a Správa datových továren a také podřízených prostředků v nich. | Ano | 
Vývojář Data Lake Analytics | Umožňuje odesílat, monitorovat a spravovat vlastní úlohy, ale neumožňuje vytvářet ani odstraňovat Data Lake Analytics účty. | Ano | 
Nástroj pro vyprázdnění dat | Může vyprázdnit analytické údaje | Ano | 
Uživatel DevTest Labs | Umožňuje připojit, spustit, restartovat a vypnout virtuální počítače ve vašem Azure DevTest Labs. | Ano | 
Přispěvatel zóny DNS | Umožňuje spravovat zóny a sady záznamů DNS v Azure DNS, ale neumožňuje řídit, kdo k nim má přístup. | Ano | 
Přispěvatel účtu DocumentDB | Může spravovat účty Azure Cosmos DB. Azure Cosmos DB se dřív jmenovala jako DocumentDB. | Ano | 
EventGrid EventSubscription Přispěvatel | Umožňuje spravovat operace odběru událostí EventGrid. | Ano | 
Čtecí modul EventSubscription EventGrid | Umožňuje číst odběry událostí EventGrid. | Ne | 
Operátor clusteru HDInsight | Umožňuje číst a upravovat konfigurace clusteru HDInsight. | Ano | 
Přispěvatel doménových služeb HDInsight | Může číst, vytvářet, upravovat a odstraňovat služby související s doménami, které jsou potřeba pro HDInsight Balíček zabezpečení podniku | Ano | 
Přispěvatel účtů inteligentních systémů | Umožňuje správu účtů inteligentních systémů, ale ne přístup k nim. | Ano | 
Přispěvatel Key Vault | Umožňuje spravovat trezory klíčů, ale ne přístup k nim. | Ano | 
Autor testovacího prostředí | Umožňuje vytvářet, spravovat a odstraňovat spravované laboratoře v rámci účtů Azure Lab. | Ano | 
Přispěvatel Log Analytics | Přispěvatel Log Analytics může číst všechna data monitorování a upravovat nastavení monitorování. Úprava nastavení monitorování zahrnuje přidání rozšíření virtuálního počítače do virtuálních počítačů. čtení klíčů účtu úložiště, aby bylo možné konfigurovat shromažďování protokolů z Azure Storage; vytváření a konfigurace účtů služby Automation; přidávání řešení; a konfigurují se diagnostiky Azure na všech prostředcích Azure. | Ano | 
Čtenář Log Analytics | Log Analytics čtenář může zobrazit a vyhledat všechna data monitorování a také zobrazit nastavení monitorování, včetně zobrazení konfigurace diagnostiky Azure na všech prostředcích Azure. | Ne | 
Přispěvatel aplikace logiky | Umožňuje spravovat Logic Apps, ale ne měnit přístup k nim. | Ano | 
Operátor aplikace logiky | Umožňuje číst, povolit a zakázat Logic Apps, ale nemůže je upravovat ani aktualizovat. | Ano | 
Role operátora spravované aplikace | Umožňuje číst a provádět akce s prostředky spravovaných aplikací. | Ano | 
Čtecí modul spravovaných aplikací | Umožňuje číst prostředky ve spravované aplikaci a vyžadovat přístup JIT. | Ne | 
Přispěvatel spravovaných identit | Vytvoření, čtení, aktualizace a odstranění identity přiřazené uživatelem | Ano | 
Spravovaný operátor identity | Čtení a přiřazení identity přiřazené uživateli | Ano | 
Přispěvatel skupiny pro správu | Role Přispěvatel skupiny pro správu | Ano | 
Čtenář skupiny pro správu | Role čtenář skupiny pro správu | Ne | 
Přispěvatel monitorování | Může číst všechna data monitorování a upravovat nastavení monitorování. Přečtěte si také téma Začínáme s rolemi, oprávněními a zabezpečením pomocí Azure Monitor. | Ano | 
Monitorování vydavatele metrik | Povoluje publikování metrik pro prostředky Azure. | Ano | 
Čtečka monitorování | Může číst všechna data monitorování (metriky, protokoly atd.). Přečtěte si také téma Začínáme s rolemi, oprávněními a zabezpečením pomocí Azure Monitor. | Ne | 
Přispěvatel sítě | Umožňuje spravovat sítě, ale ne přístup k nim. | Ano | 
Přispěvatel nového účtu Relic APM | Umožňuje správu účtů a aplikací New Relic Application Performance Management, ale ne přístup k nim. | Ano | 
Čtenář a přístup k datům | Umožňuje zobrazit vše, ale neumožní vám odstranit ani vytvořit účet úložiště nebo obsažený prostředek. Umožní taky přístup pro čtení a zápis ke všem datům, která jsou obsažená v účtu úložiště, prostřednictvím přístupu k klíčům účtu úložiště. | Ano | 
Přispěvatel Redis Cache | Umožňuje správu mezipamětí Redis, ale ne přístup k nim. | Ano | 
Přispěvatel zásad prostředků (Preview) | Tisk Uživatelé z EA mají oprávnění k vytváření a úpravám zásad prostředků, vytváření lístků podpory a čtení prostředků a hierarchie. | Ano | 
Přispěvatel kolekcí úloh Scheduleru | Umožňuje spravovat kolekce úloh Scheduleru, ale ne přístup k nim. | Ano | 
Přispěvatel Search Service | Umožňuje spravovat služby vyhledávání, ale ne přístup k nim. | Ano | 
Správce zabezpečení | Pouze v Security Center: lze zobrazit zásady zabezpečení, zobrazit stavy zabezpečení, upravit zásady zabezpečení, zobrazit výstrahy a doporučení, zavřít výstrahy a doporučení. | Ano | 
Správce zabezpečení (starší verze) | Toto je starší role. Místo toho prosím použijte Správce zabezpečení. | Ano | 
Čtenář zabezpečení | Pouze v Security Center: může zobrazit doporučení a výstrahy, zobrazit zásady zabezpečení, zobrazit stavy zabezpečení, ale nemůže provádět změny. | Ne | 
Přispěvatel Site Recovery | Umožňuje správu Site Recovery služby s výjimkou vytvoření trezoru a přiřazení role. | Ano | 
Operátor Site Recovery | Umožňuje převzetí služeb při selhání a navrácení služeb po obnovení, ale jiné operace správy Site Recovery. | Ano | 
Čtecí modul Site Recovery | Umožňuje zobrazit Site Recovery stav, ale nemůže provádět jiné operace správy. | Ne | 
Přispěvatel účtu prostorových kotev | Umožňuje spravovat prostorové kotvy ve vašem účtu, ale neodstraňovat je. | Ano | 
Vlastník účtu prostorových ukotvení | Umožňuje spravovat prostorové kotvy v účtu, včetně jejich odstranění. | Ano | 
Čtečka účtu prostorových kotev | Umožňuje vyhledat a číst vlastnosti prostorových ukotvení ve vašem účtu. | Ne | 
Přispěvatel databáze SQL | Umožňuje spravovat databáze SQL, ale ne přístup k nim. Nemůžete také spravovat zásady související se zabezpečením nebo jejich nadřazené servery SQL. | Ano | 
Přispěvatel spravované instance SQL | Umožňuje spravovat spravované instance SQL a požadovanou konfiguraci sítě, ale nemůže udělit přístup jiným uživatelům. | Ano | 
Správce zabezpečení SQL | Umožňuje spravovat zásady týkající se zabezpečení serverů a databází SQL, ale ne přístup k nim. | Ano | 
Přispěvatel SQL Server | Umožňuje spravovat servery a databáze SQL, ale ne přístup k nim, a ne jejich zásady související se zabezpečením. | Ano | 
Přispěvatel účtů úložiště | Umožňuje správu účtů úložiště. Poskytuje přístup k klíči účtu, který se dá použít pro přístup k datům přes autorizaci pomocí sdíleného klíče. | Ano | 
Role služby operátora klíče účtu úložiště | Povoluje výpis a opětovné generování přístupových klíčů účtu úložiště. | Ano | 
Přispěvatel dat v objektech blob služby Storage | Čtení, zápis a odstraňování kontejnerů Azure Storage a objektů BLOB. Chcete-li zjistit, které akce jsou pro danou datovou operaci požadovány, přečtěte si téma oprávnění pro volání operací s daty objektů BLOB a front. | Ano | 
Vlastník dat v objektech blob služby Storage | Poskytuje úplný přístup k Azure Storage kontejnerů a dat objektů blob, včetně přiřazování řízení přístupu k POSIX. Chcete-li zjistit, které akce jsou pro danou datovou operaci požadovány, přečtěte si téma oprávnění pro volání operací s daty objektů BLOB a front. | Ano | 
Čtenář dat v objektech blob služby Storage | Čtení a výpis Azure Storage kontejnerů a objektů BLOB. Chcete-li zjistit, které akce jsou pro danou datovou operaci požadovány, přečtěte si téma oprávnění pro volání operací s daty objektů BLOB a front. | Ne | 
Delegování objektu BLOB úložiště | Získejte klíč pro delegování uživatelů, který se pak dá použít k vytvoření sdíleného přístupového podpisu pro kontejner nebo objekt blob, který je podepsaný pomocí přihlašovacích údajů Azure AD. Další informace najdete v tématu Vytvoření SAS pro delegování uživatelů. | Ano | 
Přispěvatel sdílené složky SMB dat souboru úložiště | Umožňuje čtení, zápis a odstraňování přístupu v Azure Storage sdílených složkách přes SMB. | Ano | 
Přispěvatel sdílené složky SMB dat souboru úložiště s vyššími oprávněními | Umožňuje číst, zapisovat, odstraňovat a upravovat přístup k souborům NTFS v Azure Storage sdílených složkách přes SMB. | Ano | 
Čtenář sdílené složky SMB dat souboru úložiště | Povolí přístup pro čtení ke sdílené složce Azure přes SMB. | Ne | 
Přispěvatel dat fronty úložiště | Čtení, zápis a odstraňování front Azure Storage a zpráv fronty. Chcete-li zjistit, které akce jsou pro danou datovou operaci požadovány, přečtěte si téma oprávnění pro volání operací s daty objektů BLOB a front. | Ano | 
Procesor zpráv s daty ve frontě úložiště | Prohlížet, načítat a odstraňovat zprávy z Azure Storage fronty. Chcete-li zjistit, které akce jsou pro danou datovou operaci požadovány, přečtěte si téma oprávnění pro volání operací s daty objektů BLOB a front. | Ano | 
Odesílatel zprávy s daty ve frontě úložiště | Přidejte zprávy do fronty Azure Storage. Chcete-li zjistit, které akce jsou pro danou datovou operaci požadovány, přečtěte si téma oprávnění pro volání operací s daty objektů BLOB a front. | Ano | 
Čtečka dat fronty úložiště | Čtení a výpis Azure Storage front a zpráv fronty. Chcete-li zjistit, které akce jsou pro danou datovou operaci požadovány, přečtěte si téma oprávnění pro volání operací s daty objektů BLOB a front. | Ne | 
Přispěvatel žádostí o podporu | Umožňuje vytvářet a spravovat žádosti o podporu. | Ano | 
Přispěvatel Traffic Manager | Umožňuje správu profilů Traffic Manager, ale neumožňuje řídit, kdo k nim má přístup. | Ano | 
Správce uživatelských přístupů | Umožňuje spravovat přístup uživatelů k prostředkům Azure. | Ano | 
Přihlášení správce virtuálního počítače | Zobrazit Virtual Machines na portálu a přihlásit se jako správce | Ano | 
Přispěvatel virtuálních počítačů | Umožňuje správu virtuálních počítačů, ale ne přístup k nim ani k virtuální síti nebo účtu úložiště, ke kterým se připojuje. | Ano | 
Přihlášení uživatele virtuálního počítače | Zobrazte Virtual Machines na portálu a přihlaste se jako běžný uživatel. | Ano | 
Přispěvatel webového plánu | Umožňuje spravovat webové plány pro weby, ale ne přístup k nim. | Ano | 
Přispěvatel webu | Umožňuje spravovat weby (nikoli webové plány), ale ne přístup k nim. | Ano |
