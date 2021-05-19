---
title: Partnerské centrum Insights
description: Prozkoumejte tento Partnerské centrum sjednoceného řídicího panelu pro vytváření sestav. Podívejte se, jak si vedete v oblasti KPI pro prodej a nasazení, vývoj pro zákazníky a další.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: 6661fb013b25e55785dac9156e5f3561f5b50c97
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151011"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a>Partnerské centrum Insights – řídicí panel, který ukazuje, jak si vede komerční partner Microsoftu

**Odpovídající role:** Globální správce | Správce účtu | Executive report viewer | Prohlížeč sestav

## <a name="introduction"></a>Úvod

Řídicí panel Přehledy je jednotný řídicí panel pro vytváření sestav Partnerské centrum pro komerční partnery Microsoftu, kteří jsou zaregistrovaní v Microsoft Partner Network (MPN). Řídicí panel Přehledy poskytuje 360° zobrazení klíčových ukazatelů výkonu (KPI) napříč cloudovými produkty, jako jsou modely Office, Azure, Dynamics a licencování, jako jsou CSP a EA. Zpřístupňuje bohatou sadu sestav klíčových ukazatelů výkonu, které vám pomohou při rozhodování o datech ve vaší organizaci. 

## <a name="role-based-access-control-to-the-insights-dashboard"></a>Řízení přístupu na základě role k řídicímu panelu Přehledy

V systému jsou dvě nové role Partnerské centrum určené speciálně pro přístup k přehledům: **Prohlížeč sestav** a **Prohlížeč výkonných sestav.** Uživatelé v roli Executive Report Viewer mají přístup ke všem datovým sadům sestav, zatímco uživatelé s rolí Prohlížeče sestav nebudou mít přístup k citlivým datovým sadách, jako jsou výnosy a osobní údaje zákazníka/zaměstnance. 

Globální správce nebo správce účtu může přiřadit tyto role uživatelům a jsou přiřazeny buď pro celou společnost, nebo pro konkrétní umístění MPN.  

>[!Note] 
>Uživatelé, kteří byli od 20. ledna 2020 správci PROGRAMU MPN, byli automaticky přidáni do role prohlížeče sestav pro celou společnost. Mají přístup k sestavě jako k divákovi sestav bez explicitní akce, kterou vyžaduje globální správce nebo správce účtu. Globální správci nebo správci účtu mohou v případě potřeby tato přiřazení přepsat. 

## <a name="reports-available"></a>Dostupné sestavy

Následující sestavy jsou k dispozici jako součást řídicího panelu Přehledy.

**Přehled:** V sestavě přehledu se zobrazí snímek různých dostupných KPI, jako je počet zákazníků, počet aktivních předplatných, výnosy ze spotřeby Azure, aktivní licence atd.

**Zákazník**: sestava zákazníka prezentuje analýzy zákazníků, jako jsou zákaznická data o pořízení, aktivní zákazníci atd.

**Předplatné produktu**: sestava předplatných představuje analýzy získání a využití vašich cloudových předplatných (například O365, Azure, Dynamics atd.).

**Licence k produktu**: řídicí panel licence představuje licenční analýzu pro cloudové produkty založené na licencích, jako je O365, Dynamics, Power BI atd.

**Produkt – využití Azure**: Sestava využití Azure prezentuje metriky týkající se předplatných Azure vašich zákazníků, včetně výnosů a využití spotřeby Azure podle kategorií měřičů.

**Kompetence**: sestava kompetence prezentuje metriky aktivních, kvalifikovaných a rizikových kompetencí.

**Výhody**: sestava výhod představuje analytické výhody, které jste získali a využili.

## <a name="navigating-the-insights-reports"></a>Navigace v sestavách Insights

**Filtry rozsahu dat**: Výběr rozsahu dat můžete najít v pravém horním rohu každé stránky. Výstup grafů na stránce přehledu se dá přizpůsobit tak, že se vybere rozsah kalendářních dat na základě posledních 3, 6 nebo 12 měsíců nebo když vyberete vlastní rozsah kalendářních dat. Výchozí výběr rozsahu kalendářních dat je 12 měsíců. 

:::image type="content" source="images/pci/intro1.png" alt-text="Úvodní mapa":::

**Tlačítko pro zpětnou vazbu**: Každý graf nebo ovládací prvek ve všech sestavách Insights je obsažený na tlačítku pro odeslání zpětné vazby, které vám umožní zadat zpětnou vazbu instance pro funkci sestavy. 

 
**Filtry na úrovni stránky**: Kromě sestav přehled, výhody a kompetence vám všechny sestavy Insights umožňují použít filtry na úrovni stránek. 

- Vybrané filtry se použijí pro všechny grafy a metriky na stránce, včetně části Souhrn. Položka filtru bude k dispozici, pokud máte nějaká data v rámci těchto kritérií filtru. 

- Výchozí výběr každého seznamu filtru je **vše**. Pokud jste například nevybrali určitý produkt v filtr Products, výchozí výběr bude mít všechny produkty.

- Vybrané filtry se zobrazí v horní části stránky. 

:::image type="content" source="images/pci/filters.png" alt-text="Částečný snímek obrazovky s panelem Použitý filtr s výběry filtrů pro produkty, zákaznické trhy, přisuzování partnerů a prodejní kanály":::

### <a name="filters-definitions"></a>Definice filtrů:

- Produkty: Seznam všech produktů Microsoft Cloud prodaných/spravovaných vaší organizací, například O365, Azure, D365, EMS, Power BI atd.
- Zákaznické trhy: Seznam zemí zákazníků
- Atribuce partnerů: Váš typ přidružení k předplatným vašich zákazníků, například Digitální partner záznamu (DPOR), Delegované oprávnění správce (DAP) a Odkaz na správce partnera (PAL). 
- Umístění partnerů: Seznam všech umístění MPN vaší organizace.
- Prodejní kanály: Všechny prodejní kanály / ceny, přes které nakupujete/zřizujete produkty a služby, konkrétně CSP, EA, CSP indirect, Direct, Advisor, Open, others
- Segmenty zákazníků: Seznam zákaznických segmentů napříč zákaznickou základnou partnerů.

## <a name="read-about-each-of-the-dashboards-and-reports"></a>Přečtěte si o jednotlivých řídicích panelech a sestavách:

- [Partnerské centrum Insights – řídicí panel Přehled](pci-overview-report.md)

- [Partnerské centrum Insights – řídicí panel Customer](pci-customer-report.md)

- [Partnerské centrum Insights – Sestava předplatných](pci-product-subscriptions-report.md)

- [Partnerské centrum Insights – sestava licencí](pci-product-licenses-report.md)

- [Partnerské centrum Insights – sestava využití Azure](pci-azure-usage-report.md)

- [Partnerské centrum Insights – Sestava kompetencí](pci-competencies-report.md)

- [Partnerské centrum Insights – Sestava výhod](pci-benefits-report.md)
