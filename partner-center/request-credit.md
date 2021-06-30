---
title: Žádost o kredit SLA od Microsoftu
ms.topic: article
ms.date: 03/31/2021
description: Přečtěte si o výhodách, omezeních a postupech pro vyžádání kreditu smlouvy o úrovni služeb (SLA) od Microsoftu, pokud u vašich zákazníků dojde k výpadku služby.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: f521e55869d60987fb46cd5d570bf206939e0782
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080635"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Jak a kdy požádat Microsoft o kredit smlouvy o úrovni služeb (SLA)

**Odpovídající role:** Agent pro správu | Globální správce

Pokud u služby, kterou poskytujete svým zákazníkům, dojde k výpadku, můžete si od Microsoftu vyžádat kredity podle smlouvy o úrovni služeb **(SLA).**

## <a name="sla-credit-calculation"></a>Výpočet kreditu SLA

Kredity SLA od Microsoftu se určují na základě ovlivněných služeb. Pokud má například zákazník sadu Office 365, ale došlo pouze k výpadku SharePointu, kredit SLA se schválí jenom pro SharePoint, a ne pro celý plán zákazníka.

*Kredity jsou poměrné na základě ovlivněné služby a doby výpadku.* Pokud se chcete podívat na typy scénářů s nárokem na kredity SLA, podívejte se na dokument [Konsolidovaná smlouva SLA pro online služby.](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) Tyto informace platí také pro služby prodávané prostřednictvím Cloud Solution Provider (CSP).


## <a name="request-an-sla-credit"></a>Žádost o kredit SLA

*Partner CSP musí žádost a všechny požadované informace odeslat do konce kalendářního měsíce následujícího po měsíci, ve kterém došlo k incidentu.* Pokud k incidentu došlo například 15. února, Microsoft musí do 31. března přijmout žádost a všechny požadované informace. Koncoví zákazníci a nepřímí prodejci nemůže odesílat žádosti o kredit SLA. Nepřímý poskytovatel nebo partner s přímým vyúčtováním musí žádosti odesílat jejich jménem.

> [!NOTE]
> Na incidenty poradce se nárok na kredity SLA nárok nemá. Incident zveřejněný na řídicím panelu Service Health ukazuje, že může dojít k ovlivnění *tenanta,* a představuje nejlepší informace, které Microsoft měl v době publikování. Data stránky stavu představují obecnou dostupnost služby. Dopad na jednotlivé služby, omezení rizik a jejich řešení se může lišit. Další podrobnosti najdete v závěrečném příspěvku o incidentu a závěrečném závěrečném incidentu. Další [informace najdete v Microsoft 365 stavu služby.](/microsoft-365/enterprise/view-service-health#incidents-and-advisories)

### <a name="required-information"></a>Požadované informace

Ke zpracování žádosti nestačí jméno zákazníka, identifikátor tenanta, lístek partnera a časové razítko vytvoření lístku.

Před [odesláním žádosti o kredit sla](#submit-sla-credit-request)  do Microsoftu musíte shromáždit všechny následující informace, které se zahrnou do lístku podpory:

- Identifikátor GUID tenanta zákazníka
- Identifikátor [incidentu výpadku?](#outage-incident-identifier)
- Důkaz, že byl zákazník ovlivněn výpadkem a požádal o kredit sla.
- Byla ovlivněná předplatná zakoupená prostřednictvím CSP? (*ano* nebo *ne*)

#### <a name="evidence-that-proves-customer-impact"></a>Důkaz, který prokazuje dopad na zákazníky

- Informace týkající se času a doby trvání výpadku
- Počet a umístění ovlivněných uživatelů (pokud je to dostupné)
- Popisy vašich pokusů o vyřešení incidentu v době výskytu
- E-mail od ovlivněných zákazníků, který žádá o podporu, a následně o kredit
- Číslo lístku podpory a podrobnosti o kontaktu zákazníka v souvislosti s řešením dopadu na službu


#### <a name="outage-incident-identifier"></a>Identifikátor incidentu výpadku

Identifikátor incidentu výpadku najdete na stránce Service Health **v** Centrum pro správu Microsoftu 365. **ID incidentu** výpadku je číslo, před oběma písmeny zkratka, která označuje ovlivněnou službu (například *EX25194* pro výpadek Exchange Online). Následující tabulka popisuje běžné zkratky služeb:

| Dvou písmenná zkratka | Služba Microsoftu |
| ----------------------- | ----------------- |
| Ex | Exchange Online |
| FO | Ochrana Exchange Online |
| Sb | Online Skype pro firmy (dříve Lync Online) |
| Operační systém | Předplatné Office |
| PB | Power BI pro Office 365 |
| Sp | SharePoint Online |
| Ya | Yammer Enterprise |
| MO | Chyba portálu |

### <a name="submit-sla-credit-request"></a>Odeslání žádosti o kredit sla

Žádost o kredit SLA odešlete Microsoftu prostřednictvím řídicího panelu Partnerské centrum:

1. Přihlaste se k řídicímu panelu pro Partnerské centrum.
2. V nabídce vlevo zvolte Žádosti **o** služby a pak vyberte Žádosti o podporu **partnerů.**
3. Na stránce **Žádost o partnera** zvolte Nová **žádost.**
4. Na stránce **Zahájit žádost vyhledejte** oddíl **CSP – zákazníci, objednávky a předplatná.** V této části zvolte **Vyberte typ problému a** pak vyberte Žádosti o kredit služeb **zákazníkům.**
5. Na stránce **Doporučená řešení** v části Potřebujete **další pomoc?** zvolte **Ano**.
6. Na **stránce Podrobnosti** vyplňte část **Podrobnosti o** problému. Do **textového** pole Podrobnosti nezapomeňte zadat [požadované informace,](#required-information) které jste shromáždili dříve.
7. Zvolte **Odeslat a** odešlete žádost o kredit sla.

## <a name="next-steps"></a>Další kroky

- [Hlášení problémů jménem zákazníka](report-problems-on-behalf-of-a-customer.md)
