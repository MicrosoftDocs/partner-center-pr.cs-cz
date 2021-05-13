---
title: Partnerské centrum odběrů přehledů
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Podívejte se, co si vedete dobře a kde můžete zlepšit cloudová předplatná, která pro své zákazníky prodáváte nebo spravujete.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 89806b08485bc4bd286c2e14a19924ca0e281b6d
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854464"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Sestava předplatných produktů dostupná na řídicím panelu Partnerské centrum Insights

**Odpovídající role:** Globální správce | Agent správy | Prohlížeč sestav | Prohlížeč výkonných sestav

Sestava Předplatná produktů představuje analýzy cloudových předplatných, která jste prodali nebo která spravujete pro své zákazníky. Jedná se o sestavu specifickou pro produkt, která zahrnuje výkon předplatných přidružených ke cloudovým produktům, jako jsou Office 365, Azure, Dynamics a další.

Následující části si můžete prohlédnout v sestavě Předplatná produktů.

- Souhrn
- Zeměpisné rozpětí předplatných
- Trend přidávání/četnosti předplatných
- Distribuce předplatného podle umístění partnerů, prodejního kanálu, skladových tržeb, typu připojení partnera, segmentu
- Trend podle stavů předplatného
- Trend produktů

 > [!NOTE]
 > Tato sestava je k dispozici na řídicím panelu Přehledy. Pokud chcete tuto sestavu zobrazit, musíte mít přiřazenou konkrétní roli v Partnerské centrum, jako je například globální správce, správce účtu, prohlížeč sestav nebo prohlížeč sestav vedoucího pracovníka. Další informace najdete v tématu Globální správce vaší společnosti. Konkrétní typy dat v této sestavě mohou být dostupné také pro uživatele s oprávněními Executive Report Viewer.

## <a name="summary"></a>Souhrn

V souhrnné části najdete snímek klíčových ukazatelů výkonu (KPI) souvisejících s předplatným, která prodáváte nebo spravujete pro vaše zákazníky.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="souhrn sestavy předplatných":::

Další informace o jednotlivých oddílech souhrnu najdete níže:

- Předplatná:
  - Aktuální počet předplatných cloudových produktů, která prodáváte nebo spravujete.
  - Procentuální růst nebo pokles předplatných během vybraného rozsahu dat
  - Mikrograf prezentuje trend počtu předplatných předplatných v průběhu vybraného rozsahu dat měsíčně.

- Aktivní předplatná:
  - Aktuální počet odběrů cloudových produktů s aktivním využitím měřený na základě telemetrie produktů Tím se vyloučí všechna zkušební předplatná v případě předplatných Azure.
  - Procentuální nárůst nebo odmítnutí aktivních předplatných za vybrané časové období
  - Mikrograf prezentuje trend aktivních předplatných za měsíc v průběhu vybraného období.

- Přidaná předplatná:
  - Celkový počet přidaných zákaznických předplatných (prodaných nebo spravovaných) během vybraného časového období. Nová předplatná s **aktivním** nebo **obnoveným** stavem se počítají jako přidaná předplatná.
  - Procentuální nárůst nebo odmítnutí předplatných přidaných za poslední celý měsíc v porovnání s prvním celým měsícem
  - Mikrograf prezentuje měsíční trend předplatných přidaných během vybraného časového období.

- Předplatné byly v provozu:
  - Celkový počet změn zákaznických předplatných v průběhu vybraného rozsahu kalendářních dat. Předplatná s  **odloženým nebo pozastaveným** stavem v daném měsíci se počítají jako zrušené předplatné.  
  - Procento předplatných, které bylo v průběhu vybraného období změněno.
  - Mikrograf prezentuje měsíční trend předplatných, která se ve vybraném časovém období převzala.

- Předplatná podle produktů: rozpis počtu aktuálních předplatných podle cloudových produktů.

## <a name="geographical-spread-of-subscriptions"></a>Geografické rozšiřování předplatných

Zobrazení **předplatná podle geografického** zobrazení zobrazuje geografickou distribuci celkových předplatných na trzích zákazníků. Celková částka předplatného zahrnuje prodané předplatné i aktivní předplatná.

V tabulce Number of countries/region (Počet **zemí/oblastí)** se zobrazuje celkový počet zemí/oblastí, ve kterých máte předplatná, a částka za zemi celkového a aktivního předplatného.

Země v mřížce můžete vyhledat a vybrat a přiblížit tak umístění na mapě. Pokud se **chcete vrátit** k původnímu zobrazení, stiskněte na mapě možnost Domů. Najeďte myší na mapu a zobrazte všechna předplatná a aktivní předplatná podle země. Obě pole v mřížce jsou seřaditelná.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="subscriptions by geography":::

## <a name="subscription-addschurns"></a>Přidání nebo četnost změn předplatného

Toto zobrazení představuje trend předplatných. Ty jsou rozdělené do různých kategorií (Nové, Existující, Četnost změn) pro vybraný rozsah dat. Osa X představuje měsíce vybraného rozsahu dat. Osa Y představuje počet předplatných. Churned subscriptions are represented on the negative scale of the Y-axis. 

Skládaný sloupcový graf zobrazuje rozpis nových, stávajících a churnedovaných předplatných pro měsíc. Můžete znovu sestavit sloupcový graf rozdělený podle konkrétních položek zásobníku. Pokud to chcete udělat, vyberte tyto konkrétní položky v legendě. Pomocí posuvníku v horní části grafu můžete také přiblížit konkrétní období.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="přidání a četnost změn předplatného":::

## <a name="subscription-distribution"></a>Distribuce předplatného

Toto zobrazení obsahuje rozpis vašich aktuálních předplatných podle umístění MPN, segmentů zákazníků, prodejního kanálu nebo cenového modelu Azure a typu atribuce (například DPOR, DAP a další). Výběrem příslušných karet zobrazíte rozpis podle těchto kategorií. Chcete-li vytvořit výsečový graf s rozpisem konkrétních kategorií položek, vyberte tyto kategorie položek v legendě.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="distribuce předplatného":::

## <a name="subscription-state-distribution"></a>Distribuce stavu předplatného

Toto zobrazení ukazuje distribuci aktuálních zákaznických předplatných podle stavu nebo stavu předplatného. To zahrnuje následující stavy předplatného: **aktivní**, **zakázané**, **zrušení zřízení**, **otevřené**, **v období odkladu**, **uzavřené** a **jiné**.

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="distribuce stavu předplatného":::

## <a name="products-trend"></a>Trend produktů

Toto zobrazení ukazuje sloupcový graf a dva výsečové grafy. Pruhový graf prezentuje měsíční trend předplatných rozdělených podle komerčních produktů, jako je Azure, Office, Dynamics atd.

V těchto dvou výsečových grafech se zobrazuje rozpis aktuálních zákaznických předplatných. První výsečový graf rozdělí odběry podle produktů. Druhý výsečový graf rozdělí předplatná podle skladů nebo plánů. Když vyberete produkt v výsečovém grafu rozpis **podle produktů** , zobrazí se v sousedním výsečovém grafu rozpis předplatných těchto produktů pomocí SKU.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="trend produktů":::

> [!NOTE]
 > Počet předplatných rozepsaný podle SKU nemusí vždy odpovídat celkovému počtu předplatných pro daný produkt. Tato situace může nastat, pokud zákazník zakoupil více SKU v rámci stejného předplatného produktu.

## <a name="next-steps"></a>Další kroky

- Další sestavy najdete v tématu [Přehled služby partner Center](partner-center-insights.md).

>[!NOTE] 
> Nezpracovaných dat v této sestavě si můžete stáhnout z oddílu stažení sestav na řídicím panelu Insights. [Další informace](pci-download-reports.md) 
