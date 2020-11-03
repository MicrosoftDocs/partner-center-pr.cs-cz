---
title: Žádost o kredit SLA od Microsoftu
ms.topic: article
ms.date: 04/28/2020
description: Přečtěte si o výhodách, omezeních a postupech, které požadují kredity smlouvy o úrovni služeb (SLA) od Microsoftu, pokud vaši zákazníci dostanou výpadek služeb.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: cb8f6b2280318427b2015403b528fc288ef64d97
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/14/2020
ms.locfileid: "92527005"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Jak a kdy požádat o kredit smlouvy o úrovni služeb (SLA) od Microsoftu

Můžete požádat o **kredity smlouvy o úrovni služeb (SLA)** od Microsoftu v případě výpadku služby, kterou poskytujete pro vaše zákazníky.

## <a name="sla-credit-calculation"></a>Výpočet kreditu SLA

Kredity SLA od Microsoftu se stanovují na základě toho, které služby byly ovlivněny. Pokud má váš zákazník například sadu Office 365, ale jenom v případě výpadku SharePointu, je kredit SLA schválený jenom pro SharePoint a ne pro celý plán zákazníka.

*Kredity jsou ohodnocené poměrně na základě příslušné služby a doby trvání výpadku.* Typy scénářů, které jsou způsobilé pro kredity smlouvy SLA, najdete v [dokumentu SLA konsolidované služby Online Services](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). Tyto informace platí i pro služby prodávané prostřednictvím programu Cloud Solution Provider.

## <a name="request-an-sla-credit"></a>Požádat o kredit smlouvy SLA

*Partner poskytovatele Cloud Solution Provider (CSP) musí podat žádost a všechny požadované informace na konci kalendářního měsíce následujícího po měsíci, kdy došlo k incidentu.* Pokud například k incidentu došlo 15. února, společnost Microsoft musí tuto deklaraci identity a všechny požadované informace získat 31. Koncoví zákazníci a nepřímí prodejci nemůžou odesílat deklarace identity kreditu SLA; buď nepřímý poskytovatel, nebo přímý fakturační partner, musí za jeho jménem odesílat deklarace identity.

### <a name="required-information"></a>Požadované informace

Před [odesláním žádosti o kredit smlouvy SLA](#submit-sla-credit-request) společnosti Microsoft je nutné shromáždit následující informace, které chcete zahrnout do vašeho lístku podpory:

- Identifikátor GUID tenanta zákazníka
- [Identifikátor incidentu výpadku](#outage-incident-identifier)?
- Byly ovlivněná předplatná zakoupená prostřednictvím poskytovatele CSP? ( *Ano* nebo *ne* )

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

1. Přihlaste se k řídicímu panelu partnerského centra.
2. V nabídce vlevo zvolte **žádosti o služby** a pak vyberte **žádosti o podporu partnerů** .
3. Na stránce **žádost o partnera** klikněte na **nový požadavek** .
4. Na stránce **Zahájit žádost** vyhledejte část **CSP – zákazníci, objednávky a odběry** . V této části vyberte **typ problému** a pak vyberte **zákaznické služby žádosti o kredit** .
5. Na stránce **doporučená řešení** v části **potřebujete další podrobnější informace?** vyberte **Ano** .
6. Na stránce **Podrobnosti** vyplňte část **Podrobnosti o problému** . V textovém poli **Podrobnosti** Nezapomeňte zadat [požadované informace](#required-information) , které jste shromáždili dříve.
7. Kliknutím **na Odeslat** odešlete žádost o kredit smlouvy SLA.
