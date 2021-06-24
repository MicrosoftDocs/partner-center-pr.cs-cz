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
ms.openlocfilehash: cd226122f8e69e0667006f274d2ef080bbe47b9b
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565419"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Sestava předplatných produktů dostupná na řídicím panelu Partnerské centrum Insights

**Odpovídající role:** Globální správce | Agent pro správu | Prohlížeč sestav | Prohlížeč výkonných sestav

Sestava Předplatná produktů představuje analýzy cloudových předplatných, která jste prodali nebo která spravujete pro své zákazníky. Jedná se o sestavu specifickou pro produkt, která zahrnuje výkon předplatných přidružených ke cloudovým produktům, jako jsou Office 365, Azure, Dynamics a další.

Následující části si můžete prohlédnout v sestavě Předplatná produktů.

- Souhrn
- Zeměpisné rozpětí předplatných
- Trend přidávání/četnosti předplatných
- Distribuce předplatného podle umístění partnerů, prodejního kanálu, skladových tržeb, typu připojení partnera, segmentu
- Trend podle stavů předplatného
- Trend produktů

 > [!NOTE]
 > Tato sestava je k dispozici na řídicím panelu Přehledy. Pokud chcete tuto sestavu zobrazit, musíte mít přiřazenou konkrétní roli v Partnerské centrum, jako je globální správce, správce účtu, prohlížeč sestav nebo prohlížeč sestav Executive. Další informace najdete v tématu Globální správce vaší společnosti. Konkrétní typy dat v této sestavě mohou být také k dispozici pouze uživatelům s oprávněními pro zobrazení sestav Executive.

## <a name="summary"></a>Souhrn

V souhrnné části najdete snímek klíčových ukazatelů výkonu (KPI) souvisejících s předplatným, která prodáváte nebo spravujete pro vaše zákazníky.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="souhrn sestavy předplatných.":::

Další informace o jednotlivých oddílech souhrnu najdete níže:

- Předplatná:
  - Aktuální počet předplatných cloudových produktů, která prodáváte nebo spravujete.
  - Procentuální růst nebo pokles předplatných během vybraného rozsahu dat
  - Mikro chart představuje trend počtu předplatných mezi měsíci během vybraného rozsahu dat.

- Aktivní předplatná:
  - Aktuální počet odběrů cloudových produktů s aktivním využitím naměřeným na základě telemetrie produktů. Tím se vyloučí všechna zkušební předplatná pro předplatná Azure.
  - Procentuální růst nebo pokles aktivních předplatných za vybrané časové období
  - Mikro chart představuje trend aktivních předplatných od měsíce po měsících během vybraného rozsahu dat.

- Přidání předplatných:
  - Celkový počet zákaznických předplatných přidaných (prodaných nebo spravovaných) během vybraného rozsahu dat Při přidání **předplatných se** **počítají** nová předplatná se stavem Aktivní nebo Obnoveno.
  - Procentuální růst nebo pokles předplatných přidaných za poslední celý měsíc v porovnání s prvním celým měsícem
  - Mikro chart představuje měsíční trend předplatných přidaných během vybraného rozsahu dat.

- Četnost změn předplatných:
  - Total customer subscriptions churned during your selected date range. Předplatná se  **stavem Zrušeno nebo** Pozastaveno se v tomto měsíci počítají jako churned subscription (Předplatné se zrušeno nebo pozastaveno).  
  - Procento předplatných, která se během vybraného rozsahu dat četnosti změn
  - Mikro chart představuje měsíční trend předplatných, která se ve vybraném rozsahu dat pohybují.

- Předplatná podle produktů: Rozpis aktuálního počtu předplatných podle cloudových produktů.

## <a name="geographical-spread-of-subscriptions"></a>Zeměpisné rozpětí předplatných

Zobrazení **Předplatná podle geografických** oblastí zobrazují zeměpisné rozdělení celkového počtu předplatných podle zákaznických trhů. Celková částka předplatného zahrnuje prodané i aktivní předplatná.

Tabulka Number of countries/region (Počet **zemí/oblastí)** uvádí celkový počet zemí/oblastí, ve kterých máte předplatná, a částka za zemi celkového a aktivního předplatného.

Země v mřížce můžete vyhledat a vybrat a přiblížit tak umístění na mapě. Pokud se **chcete vrátit** k původnímu zobrazení, stiskněte na mapě možnost Domů. Najeďte myší na mapu a zobrazte všechna předplatná a aktivní předplatná podle země. Obě pole v mřížce jsou seřaditelná.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="subscriptions by geography.":::

## <a name="subscription-addschurns"></a>Přidání nebo četnost změn předplatného

Toto zobrazení představuje trend předplatných. Ty jsou rozdělené do různých kategorií (Nové, Existující, Četnost změn) pro vybraný rozsah dat. Osa X představuje měsíce vybraného rozsahu dat. Osa Y představuje počet předplatných. Churned subscriptions are represented on the negative scale of the Y-axis. 

Skládaný sloupcový graf zobrazuje rozpis nových, stávajících a churnedovaných předplatných pro měsíc. Můžete znovu sestavit sloupcový graf rozdělený podle konkrétních položek zásobníku. Pokud to chcete udělat, vyberte tyto konkrétní položky v legendě. Pomocí posuvníku v horní části grafu můžete také přiblížit konkrétní období.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="subscription adds and churns.":::

## <a name="subscription-distribution"></a>Distribuce předplatného

Toto zobrazení představuje rozpis vašich aktuálních předplatných podle umístění Microsoft Partner Network (MPN), zákaznických segmentů, prodejního kanálu nebo cenového modelu Azure a typu atribuce. Výběrem příslušných karet zobrazíte rozpis podle těchto kategorií. Pokud chcete vytvořit výsečový graf s rozpisem kategorií konkrétních položek, vyberte tyto kategorie položek v legendě.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="distribuce předplatného.":::

## <a name="subscription-state-distribution"></a>Distribuce stavu předplatného

Toto zobrazení ukazuje distribuci aktuálních zákaznických předplatných podle stavu nebo stavu předplatného. To zahrnuje následující stavy předplatného: **Aktivní,** **Zakázáno,** **Zrušeno** zřízení, **Otevření,** V obdobíchová období, **Uzavřeno** **a další.** 

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="distribuce stavu předplatného.":::

## <a name="products-trend"></a>Trend produktů

Toto zobrazení zobrazuje pruhový graf a dva výsečové grafy. Pruhový graf představuje měsíční trend předplatných rozdělených podle komerčních produktů, jako jsou Azure, Office a Dynamics.

Dva výsečové grafy zobrazují rozpis vašich aktuálních zákaznických předplatných. První výsečový graf rozdělí předplatná podle produktů. Druhý výsečový graf rozdělí předplatná podle SKU nebo plánů. Když vyberete produkt ve výsečovém grafu **Products** (Produkty), zobrazí se v sousedním výsečovém grafu rozpis předplatných tohoto produktu podle SKU.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="trend produktů.":::

> [!NOTE]
 > Počet předplatných rozdělený podle SKU nemusí vždy odpovídat celkovému počtu předplatných pro tento produkt. K tomu může dojít v případě, že zákazník v rámci stejného předplatného produktu zakoupil více SKU.

## <a name="next-steps"></a>Další kroky

- Další sestavy najdete v tématu [Partnerské centrum Insights.](partner-center-insights.md)

>[!NOTE] 
> Nezpracovaná data pohánějící tuto sestavu si můžete stáhnout z části Stažení sestav na řídicím panelu Přehledy. [Další informace](pci-download-reports.md) 
