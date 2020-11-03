---
title: Přehledy partnerského centra
description: Prozkoumejte tento řídicí panel pro jednotný oznamovací centrum pro partnery. Podívejte se, jak se v klíčových ukazatelích výkonu provádí prodej a nasazení, zákaznická vývoj a další.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: 2b1a09253b7a9e9c8863f07b729ad116689a4642
ms.sourcegitcommit: bcd0c09d3acd5eae4fbfca7ea6614a54d203eff6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/04/2020
ms.locfileid: "92527228"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a>Přehledy partnerského centra – řídicí panel, který ukazuje, jak probíhá komerční partner Microsoftu

**Příslušné role**
- Globální správce
- Správce účtu
- Prohlížeč sestav Executive
- Prohlížeč sestav

## <a name="introduction"></a>Úvod

Insights je jednotný řídicí panel pro vytváření sestav v partnerském centru pro komerční partnery Microsoftu, kteří jsou zaregistrovaní v programu Microsoft Partner Network (MPN). Řídicí panel Insights poskytuje zobrazení klíčových ukazatelů výkonu (KPI) v různých cloudových produktech, jako jsou například CSP a EA, 360. Zpřístupňuje bohatou sadu sestav klíčových ukazatelů výkonu, které vám můžou usnadnit rozhodování na základě dat ve vaší organizaci. 

## <a name="role-based-access-control-to-the-insights-dashboard"></a>Řízení přístupu na základě role na řídicí panel Insights

V partnerském centru jsou dvě nové role navržené speciálně pro přístup k přehledům: **Prohlížeč sestav** a **manažer sestav v nástroji Executive** . Uživatelé v roli manažer sestav vedoucí mají přístup ke všem datovým sadám sestav, zatímco uživatelé v roli prohlížeče sestav nebudou mít přístup k citlivým datovým sadám, jako jsou výnosy a osobní údaje zákazníka/zaměstnance. 

Globální správce nebo správce účtu může přiřadit uživatele k těmto rolím a přiřadí se buď pro celou firmu, nebo pro konkrétní umístění MPN.  

>[!Note] 
>Uživatelé, kteří byli správci MPN od 20. ledna 2020, byli automaticky přidáni do role prohlížeče sestav v rámci společnosti. Budou mít přístup k sestavám jako Prohlížeč sestav bez jakékoli explicitní akce vyžadované správcem globálního správce nebo účtu. Globální správci nebo správci účtu můžou Tato přiřazení v případě potřeby přepsat. 

## <a name="reports-available"></a>Dostupné sestavy

V rámci řídicího panelu Insights jsou k dispozici následující sestavy.

**Přehled** : Sestava přehledu představuje zobrazení snímku různých klíčových ukazatelů výkonu, které vás zajímají, jako je počet zákazníků, počet aktivních předplatných, výnosy za využití Azure, aktivní licence atd.

**Zákazník** : sestava zákazníka prezentuje analýzy zákazníků, jako jsou zákaznická data o pořízení, aktivní zákazníci atd.

**Předplatné produktu** : sestava předplatných představuje analýzy získání a využití vašich cloudových předplatných (například O365, Azure, Dynamics atd.).

**Licence k produktu** : řídicí panel licence představuje licenční analýzu pro cloudové produkty založené na licencích, jako je O365, Dynamics, Power BI atd.

**Produkt – využití Azure** : Sestava využití Azure prezentuje metriky týkající se předplatných Azure vašich zákazníků, včetně výnosů a využití spotřeby Azure podle kategorií měřičů.

**Kompetence** : sestava kompetence prezentuje metriky aktivních, kvalifikovaných a rizikových kompetencí.

**Výhody** : sestava výhod představuje analytické výhody, které jste získali a využili.

## <a name="navigating-the-insights-reports"></a>Navigace v sestavách Insights

**Filtry rozsahu dat** : Výběr rozsahu dat můžete najít v pravém horním rohu každé stránky. Výstup grafů na stránce přehledu se dá přizpůsobit tak, že se vybere rozsah kalendářních dat na základě posledních 3, 6 nebo 12 měsíců nebo když vyberete vlastní rozsah kalendářních dat. Výchozí výběr rozsahu kalendářních dat je 12 měsíců. 

:::image type="content" source="images/pci/intro1.png" alt-text="Úvodní mapa":::

**Tlačítko pro zpětnou vazbu** : Každý graf nebo ovládací prvek ve všech sestavách Insights je obsažený na tlačítku pro odeslání zpětné vazby, které vám umožní zadat zpětnou vazbu instance pro funkci sestavy. 

 
**Filtry na úrovni stránky** : Kromě sestav přehled, výhody a kompetence vám všechny sestavy Insights umožňují použít filtry na úrovni stránek. 

- Vybrané filtry se použijí pro všechny grafy a metriky na stránce, včetně části Souhrn. Položka filtru bude k dispozici, pokud máte nějaká data v rámci těchto kritérií filtru. 

- Výchozí výběr každého seznamu filtru je **vše** . Pokud jste například nevybrali určitý produkt v filtr Products, výchozí výběr bude mít všechny produkty.

- Vybrané filtry se zobrazí v horní části stránky. 

:::image type="content" source="images/pci/filters.png" alt-text="Úvodní mapa":::

### <a name="filters-definitions"></a>Definice filtrů:

- Produkty: seznam všech produktů Microsoft Cloud prodaných/spravovaných vaší organizací, například O365, Azure, D365, EMS, Power BI atd.
- Trhy zákazníka: seznam zemí zákazníka
- Vlastnictví partnerů: typ přidružení s předplatnými vašich zákazníků, například digitální partner záznamu (partnera DPOR), delegované oprávnění správce (DAP), partnerský odkaz pro správu (PAL) atd. 
- Umístění partnerů: seznam všech umístění programu MPN vaší organizace.
- Prodejní kanály: veškerý prodejní kanál nebo ceny, pomocí kterých si koupíte/zřídíte produkty a služby, jako je CSP, EA, zprostředkovatel CSP, přímý, přímý, poradce, otevřený, ostatní
- Zákaznické segmenty: seznam zákaznických segmentů napříč zákaznickou základnou pro partnery.

## <a name="read-about-each-of-the-dashboards-and-reports"></a>Přečtěte si o jednotlivých řídicích panelech a sestavách:

- [Přehled partnerského centra – přehled](pci-overview-report.md)

- [Přehledy partnerského centra – řídicí panel zákazníka](pci-customer-report.md)

- [Sestava partnerů – přehledy – předplatná](pci-product-subscriptions-report.md)

- [Sestava pro partnery – Přehled licencí](pci-product-licenses-report.md)

- [Přehled služby partner Center – sestava využití Azure](pci-azure-usage-report.md)

- [Sestava pro partnery – přehled kompetencí](pci-competencies-report.md)

- [Sestava o výhodách pro partnery – přehled](pci-benefits-report.md)
