---
title: Žádost o kredit SLA od Microsoftu
ms.topic: article
ms.date: 03/31/2021
description: Přečtěte si o výhodách, omezeních a postupech, které požadují kredity smlouvy o úrovni služeb (SLA) od Microsoftu, pokud vaši zákazníci dostanou výpadek služeb.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 1046d8afc8889461f75fb4c837d0e5af94c13e9f
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018148"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Jak a kdy požádat o kredit smlouvy o úrovni služeb (SLA) od Microsoftu

**Příslušné role**

- Agent správce
- Globální správce

**Kredity smlouvy o úrovni služeb (SLA)** si můžete vyžádat od Microsoftu, pokud služba, kterou poskytujete pro vaše zákazníky, má výpadek.

## <a name="sla-credit-calculation"></a>Výpočet kreditu SLA

Kredity SLA od Microsoftu se stanovují na základě toho, které služby byly ovlivněny. Pokud má váš zákazník například sadu Office 365, ale jenom v případě výpadku SharePointu, je kredit SLA schválený jenom pro SharePoint a ne pro celý plán zákazníka.

*Kredity jsou ohodnocené poměrně na základě příslušné služby a doby trvání výpadku.* Typy scénářů, které jsou způsobilé pro kredity smlouvy SLA, najdete v [dokumentu SLA konsolidované služby Online Services](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). Tyto informace platí i pro služby prodávané prostřednictvím programu Cloud Solution Provider.


## <a name="request-an-sla-credit"></a>Požádat o kredit smlouvy SLA

*Partner poskytovatele Cloud Solution Provider (CSP) musí podat žádost a všechny požadované informace na konci kalendářního měsíce následujícího po měsíci, kdy došlo k incidentu.* Například pokud k incidentu došlo 15. února, společnost Microsoft musí tuto deklaraci identity a všechny požadované informace získat do 31. března. Koncoví zákazníci a nepřímí prodejci nemůžou odesílat deklarace identity kreditu SLA; buď nepřímý poskytovatel, nebo přímý fakturační partner, musí za jeho jménem odesílat deklarace identity.

>[!NOTE]
>Poradenské incidenty ([Jak kontrolovat Microsoft 365 Service Health](https://docs.microsoft.com/microsoft-365/enterprise/view-service-health?&preserve-view=trueo365-worldwide#incidents-and-advisories)) nemají nárok na kredity smlouvy SLA.

### <a name="required-information"></a>Požadované informace

Název zákazníka, identifikátor tenanta, ID partnerského lístku a datum a časové razítko vytvořeného lístku nejsou dostačující pro zpracování deklarace identity.

Před [odesláním žádosti o kredit smlouvy SLA](#submit-sla-credit-request) společnosti Microsoft je nutné shromáždit **všechny** následující informace, které chcete zahrnout do vašeho lístku podpory:

- Identifikátor GUID tenanta zákazníka
- [Identifikátor incidentu výpadku](#outage-incident-identifier)?
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
| SP | SharePoint Online |
| DOLŮ | Yammer Enterprise |
| MO | Chyba portálu |

### <a name="submit-sla-credit-request"></a>Odeslat žádost o kredit SLA

Odeslání žádosti o kredit SLA společnosti Microsoft prostřednictvím řídicího panelu partnerského centra:

1. Přihlaste se k řídicímu panelu pro Partnerské centrum.
2. V nabídce vlevo zvolte **žádosti o služby** a pak vyberte **žádosti o podporu partnerů**.
3. Na stránce **žádost o partnera** klikněte na **nový požadavek**.
4. Na stránce **Zahájit žádost** vyhledejte část **CSP – zákazníci, objednávky a odběry**. V této části vyberte **typ problému** a pak vyberte **zákaznické služby žádosti o kredit**.
5. Na stránce **doporučená řešení** v části **potřebujete další podrobnější informace?** vyberte **Ano**.
6. Na stránce **Podrobnosti** vyplňte část **Podrobnosti o problému** . V textovém poli **Podrobnosti** Nezapomeňte zadat [požadované informace](#required-information) , které jste shromáždili dříve.
7. Kliknutím **na Odeslat** odešlete žádost o kredit smlouvy SLA.

## <a name="next-steps"></a>Další kroky

- [Nahlásit problémy jménem zákazníka](report-problems-on-behalf-of-a-customer.md)
