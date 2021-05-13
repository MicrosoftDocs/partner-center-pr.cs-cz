---
title: Řídicí panel výkonu služby partner Center Insights pro prodejce
ms.topic: article
ms.date: 09/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Řídicí panel výkon prodejce v partnerském centru přehledy poskytuje přehled o výkonu různých nepřímých prodejců nepřímých poskytovatelů CSP.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a2a5697f19baadb5af956a745c032ce1711574d3
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855229"
---
# <a name="reseller-performance-dashboard-in-partner-center-insights"></a>Řídicí panel výkonu prodejce ve službě partner Center – přehledy

**Příslušné role**: globální správce | Agent správce | Prohlížeč sestav | Prohlížeč sestav Executive

Řídicí panel výkon prodejce v partnerském centru přehledy poskytuje přehled o výkonu různých nepřímých prodejců nepřímých poskytovatelů CSP. Řídicí panel poskytuje data prodejcům, kteří jsou aktivní, kolik výnosů vygenerovalo a jaké produkty řídí výnosy. Nepřímá poskytovatelé budou moci vyhledat konkrétního prodejce podle názvu a vyhledat podrobnosti pro prodejce na řídicím panelu výkonu prodejce.

Následující části můžete zobrazit na řídicím panelu výkonu prodejce.

- Souhrn
- Geografické rozšiřování prodejců
- Prodejci přidávají/změn 
- Trend příjmů prodejců 
- Výkon prodejců podle produktů
- Aktivní prodejci podle umístění partnerů
- Trend geografické distribuce výnosů
- Výkon prodejce podle zákaznického segmentu
- Stav podepisování aktivace prodejce

 > [!NOTE]
 > Tato sestava je k dispozici na řídicím panelu Insights. Pokud chcete zobrazit tuto sestavu, musíte mít přiřazenou konkrétní roli v partnerském centru, jako je například globální správce, správce účtu, Prohlížeč sestav nebo správce sestav v nástroji Executive. Další informace najdete v tématu globální správce vaší společnosti. konkrétní typy dat v této sestavě mohou být také k dispozici pouze uživatelům s oprávněními správce sestav nástroje Executive.

## <a name="summary"></a>Souhrn

V části Souhrn se zobrazuje snímek klíčových ukazatelů výkonu (KPI) souvisejících s nepřímým zprostředkovatelem CSP.

- Aktivní prodejci: Počet prodejců, kteří mají během tohoto měsíce alespoň jedno aktivní předplatné.

Mikro chart představuje trend od měsíce po měsíci u různých prodejců, kteří byli aktivní ve vybraném rozsahu dat.

- Prodejci transakcí: Počet prodejců, kteří během tohoto měsíce prodali alespoň jedno předplatné. 

Mikro chart představuje trend prodejců zaregistrovaých pro vybraný rozsah dat mezi měsíci.

- Noví prodejci: Počet prodejců, kteří v průběhu tohoto měsíce začali s nepřímým poskytovatelem provádět transakce. 

Mikro chart představuje trend celkového počtu nových prodejců za měsíc po měsících ve vybraném rozsahu dat.

- Billed revenue USD: Revenue in USD driven by the resellers during that month. 

Mikro chart představuje trend tržeb mezi měsíci během vybraného rozsahu dat.

- Oddíl Billed revenue by products (Fakturované výnosy podle produktů) poskytuje měsíční rozpis fakturovaných výnosů v USD v dělení podle prodaných produktů. 

:::image type="content" source="images/pci/pci-res-perf-summary-1.png" alt-text="resellers performance summary":::

## <a name="geographical-spread-of-resellers"></a>Zeměpisné rozpětí prodejců

Zobrazení **Resellers by geography (Prodejci podle zeměpisné oblasti) poskytuje geografickou distribuci prodejců. Pomocí tohoto widgetu mohou partneři zobrazit **celkový** počet prodejců, nových prodejců a fakturovaných výnosů **(USD)** rozdělených podle různých zeměpisných lokalit.

Země v mřížce můžete vyhledat a vybrat a přiblížit tak umístění na mapě. Pokud se **chcete vrátit** k původnímu zobrazení, stiskněte na mapě možnost Domů. Najeďte myší na mapu a zobrazte **fakturované výnosy (USD)** podle země. Pole Billed Revenue (USD) (Fakturované výnosy) v mřížce je seřaditelné.

:::image type="content" source="images/pci/pci-res-perf-resel-by-geo-1.png" alt-text="Prodejci podle zeměpisné oblasti ":::

## <a name="resellers-addchurns"></a>Maloobchodníci přidávají/četnosti změn

Toto zobrazení poskytuje měsíční rozdělení počtu nových prodejců, **churned resellers** a **stávajících prodejců.** 

- Noví prodejci: počet prodejců, kteří byli nově zaregistrovaní v nepřímém poskytovateli během vybraného rozsahu kalendářních dat.
- Změněný prodejci: počet prodejců, kteří za posledních šest měsíců neprošli transakcí s výjimkou aktuálního měsíce.
- Stávající prodejci: počet prodejců, kteří v předchozím měsíci používali transakce.

:::image type="content" source="images/pci/pci-res-perf-resel-add-churn-1.png" alt-text="Prodejci přidávají/změn":::

## <a name="resellers-revenue-trend"></a>Trend příjmů prodejců 

Toto zobrazení poskytuje měsíční trend fakturovaných výnosů (USD) rozdělených podle produktů, konkrétně O365, D365, EMS, Power BI a Azure. Celkové metriky jsou shrnuté napříč různými produkty pro každý měsíc. Partner může vyhledat konkrétního prodejce podle názvu a vyhledat data tohoto konkrétního prodejce. Pole účtované tržby (USD) v mřížce je seřaditelné.

:::image type="content" source="images/pci/pci-res-perf-resel-rev-trend-1.png" alt-text="Trend příjmů prodejců":::

## <a name="reseller-performance-by-products"></a>Výkon prodejců podle produktů

Toto zobrazení poskytuje rozdělení klíčových metrik, jako jsou účtované tržby, počet předplatných a počet licencí podle různých produktů v měsíci na základě měsíce. Výsečový graf na pravé straně indikuje celkové rozdělení metrik podle různých produktů, takže partner získá rychlou nakouknětei rozložení podle různých produktů, které prodejce prodává.

:::image type="content" source="images/pci/pci-res-perf-resel-perf-product-1.png" alt-text="Výkon prodejců podle produktů":::

## <a name="active-resellers-by-partner-locations"></a>Aktivní prodejci podle umístění partnerů

Toto zobrazení poskytuje rozdělení aktivních prodejců podle geografických oblastí partnerů. V legendě vidíte horních pět geografických oblastí a zbývající je zařazená do kategorie jiné.

:::image type="content" source="images/pci/pci-res-perf-part-loc-1.png" alt-text="Aktivní prodejci podle umístění partnerů":::

## <a name="revenue-geo-distribution-trend"></a>Trend geografické distribuce výnosů

Toto zobrazení poskytuje trend měsíčního obratu fakturovaných výnosů (USD), které je rozdělené do pěti hlavních geografických oblastí.  Zbytek výnosů je zařazený do kategorie Ostatní.

:::image type="content" source="images/pci/pci-res-perf-rev-geo-trend-1.png" alt-text="Trend geografické distribuce výnosů":::

## <a name="reseller-performance-by-customer-segment"></a>Výkon prodejce podle segmentu zákazníků

Toto zobrazení umožňuje partnerovi porozumět měsíčnímu trendu výnosů v USD, počtu předplatných a licencí rozdělených podle různých zákaznických segmentů. V grafu se zobrazuje pět nejlepších segmentů zákazníků a zbývající segmenty jsou zařazené do kategorie Ostatní.

:::image type="content" source="images/pci/pci-res-perf-resel-cust-seg-1.png" alt-text="Výkon prodejce podle segmentu zákazníků":::

## <a name="reseller-mpa-signing-status"></a>Stav podepsání smlouvy MPA prodejce

Toto zobrazení poskytuje stav podepisování SMLOUVY MPA pro prodejce spolu s dalšími metadaty, jako je stav prověřování MPN, stav migrace PMC do POČÍTAČE atd.

:::image type="content" source="images/pci/pci-res-perf-mpa-stat-1.png" alt-text="Stav podepsání smlouvy MPA prodejce":::

## <a name="next-steps"></a>Další kroky

- Další sestavy najdete v tématu [Partnerské centrum Insights.](partner-center-insights.md)

>[!NOTE] 
> Nezpracovaná data pohánějící tuto sestavu si můžete stáhnout z části Stažení sestav na řídicím panelu Přehledy. [Další informace](pci-download-reports.md) 
