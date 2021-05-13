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
ms.openlocfilehash: 74dd5c2c9457961f07dd0dd8d5a6ead9047c5579
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855552"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Jak a kdy požádat Microsoft o kredit smlouvy o úrovni služeb (SLA)

**Odpovídající role:** Agent pro správu | Globální správce

Pokud u služby, kterou poskytujete svým zákazníkům, dojde k výpadku, můžete si od Microsoftu vyžádat kredity podle smlouvy o úrovni služeb **(SLA).**

## <a name="sla-credit-calculation"></a>Výpočet kreditu SLA

Kredity SLA od Microsoftu se určují na základě ovlivněných služeb. Pokud má například zákazník sadu Office 365, ale došlo pouze k výpadku SharePointu, kredit SLA se schválí jenom pro SharePoint, a ne pro celý plán zákazníka.

*Kredity jsou poměrné na základě ovlivněné služby a doby výpadku.* Pokud se chcete podívat na typy scénářů s nárokem na kredity SLA, podívejte se na dokument [Konsolidovaná smlouva SLA pro online služby.](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) Tyto informace platí i pro služby prodávané Cloud Solution Provider programu.


## <a name="request-an-sla-credit"></a>Žádost o kredit SLA

*Partner Cloud Solution Provider (CSP) musí žádost a všechny požadované informace odeslat do konce kalendářního měsíce následujícího po měsíci, ve kterém k incidentu došlo.* Pokud k incidentu došlo například 15. února, Microsoft musí do 31. března přijmout žádost a všechny požadované informace. Koncoví zákazníci a nepřímí prodejci nemůže odesílat žádosti o kredit SLA. Nepřímý poskytovatel nebo partner s přímým vyúčtováním musí žádosti odesílat jejich jménem.

>[!NOTE]
>Poradce pro incidenty ([Postup kontroly Microsoft 365 service health](https://docs.microsoft.com/microsoft-365/enterprise/view-service-health?&preserve-view=trueo365-worldwide#incidents-and-advisories)) nemají nárok na kredity SLA.

### <a name="required-information"></a>Požadované informace

Ke zpracování žádosti nestačí jméno zákazníka, identifikátor tenanta, lístek partnera a časové razítko vytvoření lístku.

Před [odesláním žádosti o kredit sla](#submit-sla-credit-request)  do Microsoftu musíte shromáždit všechny následující informace, které se zahrnou do lístku podpory:

- Identifikátor GUID tenanta zákazníka
- Identifikátor [incidentu výpadku](#outage-incident-identifier)?
- Důkaz, že zákazník ovlivnil výpadek a požadoval kredit SLA.
- Byly ovlivněná předplatná zakoupená prostřednictvím poskytovatele CSP? (*Ano* nebo *ne*)

#### <a name="evidence-that-proves-customer-impact"></a>Důkaz, který ukáže dopad na zákazníky

- Informace týkající se času a doby trvání výpadku
- Počet a umístění ovlivněných uživatelů (Pokud je k dispozici)
- Popisy vašich pokusů o vyřešení incidentu v době výskytu
- E-mail od ovlivněného zákazníka žádající o podporu a následně dal
- Číslo lístku podpory a podrobnosti kontaktu zákazníka v souvislosti s řešením dopadu služby


#### <a name="outage-incident-identifier"></a>Identifikátor incidentu výpadku

Identifikátor incidentu výpadku najdete na stránce **Service Health** v centru pro správu Microsoft 365. **ID incidentu výpadku** je číslo předchází zkratkou se dvěma písmeny, která označuje ovlivněnou službu (například *EX25194* výpadku Exchange Online). V následující tabulce jsou popsány běžné zkratky pro služby:

| Zkratka se dvěma písmeny | Služba Microsoftu |
| ----------------------- | ----------------- |
| DODATEČNÉ | Exchange Online |
| FO | Ochrana systému Exchange Online |
| SB | Online Skype pro firmy (dřív Lync Online) |
| Operační systém | Předplatné Office |
| PB | Power BI pro Office 365 |
| Sp | SharePoint Online |
| Ya | Yammer Enterprise |
| MO | Chyba portálu |

### <a name="submit-sla-credit-request"></a>Odeslání žádosti o kredit sla

Žádost o kredit sla odešlete Microsoftu prostřednictvím řídicího panelu Partnerské centrum:

1. Přihlaste se k řídicímu panelu pro Partnerské centrum.
2. V nabídce vlevo zvolte Žádosti **o** služby a pak vyberte **Žádosti o podporu partnerů.**
3. Na stránce **Žádost o partnera** zvolte Nová **žádost.**
4. Na stránce **Zahájit žádost vyhledejte** oddíl **CSP – zákazníci, objednávky a předplatná.** V této části zvolte **Vyberte typ problému a** pak vyberte Žádosti o kredit služeb **zákazníkům.**
5. Na stránce **Doporučená řešení** v části Potřebujete **další pomoc?** zvolte **Ano**.
6. Na **stránce Podrobnosti** vyplňte část **Podrobnosti o** problému. Do **textového** pole Podrobnosti zadejte [](#required-information) požadované informace, které jste shromáždili dříve.
7. Zvolte **Odeslat a** odešlete žádost o kredit sla.

## <a name="next-steps"></a>Další kroky

- [Hlášení problémů jménem zákazníka](report-problems-on-behalf-of-a-customer.md)
