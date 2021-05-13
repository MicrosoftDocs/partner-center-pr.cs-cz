---
title: Řídicí panel přehled služby partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Podívejte se na snímek toho, jak provádíte s prodejem a nasazením, růstem zákazníků a růstem výnosů s licencemi, předplatnými a využitím Azure.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e274b0a637c7fd4944a395ba7e38154e36d2a9e3
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855195"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>Přehled sestav řídicích panelů dostupných ve službě partner Center – přehledy
 
**Příslušné role**: globální správce | Agent správce | Prohlížeč sestav | Prohlížeč sestav Executive

Řídicí panel přehled Insights nabízí zobrazení snímků klíčových ukazatelů výkonu, jako jsou zákazníci, předplatná, výnosy za využití Azure a licence. V sestavě přehledu můžete vizualizovat následující grafy.

- Souhrn  
- Geografické rozšiřování vašich zákazníků, předplatných a licencí  
- Trend růstu pro zákazníky 
- Geometrický trend předplatných 
- Trend růstu spotřebovaných výnosů v Azure 
- Trend růstu licencí 

## <a name="summary"></a>Souhrn

Souhrn obsahuje informace o zákaznících, výnosech spotřebovaných v Azure (ACR), prodávaných předplatných, aktivních předplatných a licencích. 

:::image type="content" source="images/pci/summary.png" alt-text="Souhrnné licence":::

Další informace o jednotlivých částech souhrnu najdete v tématu.

### <a name="customers"></a>Zákazníci

Oblast **zákazníci** zahrnuje:

- Aktuální počet všech zákazníků s alespoň jedním aktivním předplatným přidruženým k vaší firmě prostřednictvím různých typů přiřazení a všech cloudových produktů.
- Procentuální nárůst počtu zákazníků v průběhu vybraného období.
- Mikrograf prezentuje trend počtu zákazníků v měsíci v rámci vybraného rozsahu kalendářních dat.

### <a name="azure-consumed-revenue-acr"></a>Tržby spotřebované za Azure (ACR)

Oblast **Azure spotřebované tržby (ACR)** na souhrnu zahrnuje:

- Celkový počet výnosy z využití Azure (v USD $) přisuzovaný vám za vybraný rozsah dat.
- Procento růstu nebo poklesu atribuce ACR (v USD) během vybraného rozsahu dat
- Mikro chart představuje měsíční trend ACR US$ přidělovaný vám ve vybraném rozsahu dat. 

> [!NOTE]
> výnosy z využití Azure (ACR) jsou dostupná pro uživatele, kteří mají přiřazenou roli Prohlížeče výkonných sestav. 
 
### <a name="subscriptions-sold"></a>Prodané předplatná

Oblast **Subscriptions sold** (Prodané předplatná) v části Summary (Souhrn) zahrnuje:

- Celkový aktuální počet předplatných cloudových produktů (aktivních a neaktivních), která prodáváte nebo spravujete vy.  
- Procentuální růst nebo pokles předplatných během vybraného rozsahu dat
- Mikro chart představuje trend celkového počtu předplatných za měsíc v rámci vybraného rozsahu dat.

### <a name="active-subscriptions"></a>Aktivní předplatná

Oblast **Aktivní předplatná** v části Souhrn zahrnuje:

- Aktuální počet předplatných cloudových produktů s aktivním využitím měřený na základě telemetrie produktů. V případě předplatných Azure se vyloučí všechna zkušební předplatná.  
- Procentuální růst aktivních předplatných ve vybraném rozsahu dat
- Mikro chart představuje trend aktivních předplatných od měsíce po měsících ve vybraném rozsahu dat.
 
### <a name="licenses-deployed"></a>Nasazené licence

Oblast **Licence nasazené** v souhrnu zahrnuje:
 
- Počet všech licencí cloudových produktů nasazených ve vašich předplatných zákazníků během vybraného časového období. 
- Procentuální růst nebo pokles těchto licencí během vybraného rozsahu dat. 
- Mikro graf ukazuje trend těchto přiřazených licencí po měsících v průběhu vybraného rozsahu dat.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Geografické rozšiřování vašich zákazníků, předplatných a licencí

Toto zobrazení je geografickou distribucí celkových zákazníků, předplatných a licencí podle země zákazníka. Výběrem různých karet zobrazíte všechny tyto přehledy na mapě. Můžete vyhledat a vybrat zemi v mřížce pro přiblížení do umístění v mapě. Kliknutím na tlačítko domů na mapě se vraťte k původnímu zobrazení. Po kliknutí na jednotlivé karty (například zákazníci, předplatná) se zobrazí hodnota metriky pro každou zemi a procento celku pro danou zemi.  

:::image type="content" source="images/pci/geosummary.png" alt-text="Zeměpisný souhrn":::

## <a name="customers-growth-trend"></a>Trend růstu pro zákazníky

Pro vybraný rozsah dat se počítá měsíční trend z celkového počtu zákazníků. Osa X představuje měsíce vybraného rozsahu kalendářních dat a osa Y představuje celkový počet zákazníků pro daný měsíc. 

:::image type="content" source="images/pci/customergrowth.png" alt-text="trend růstu pro zákazníky":::

## <a name="subscriptions-growth-trend"></a>Geometrický trend předplatných

To indikuje trend počtu předplatných zákazníků pro vybraný rozsah kalendářních dat. Osa X představuje měsíce vybraného rozsahu kalendářních dat a osa Y představuje počet předplatných vybraných pro daný produkt. Posuňte se přes posuvník nad grafem, aby se graf zvětšil na konkrétní časové období. 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="Trend růstu předplatného":::

## <a name="azure-consumed-revenue-growth-trend"></a>Trend růstu spotřebovaných výnosů v Azure

Měsíční trend využívání Azure s využitím výnosů, který je na vás za vybraným rozsahem dat. Osa X představuje měsíce vybraného rozsahu kalendářních dat a osa Y představuje celkový počet zpracovaných výnosů v Azure, které vám za tento měsíc platil.

> [!NOTE]
> Výnosy za Azure (ACR) budou viditelné jenom uživatelům, kterým byla přiřazena role vedoucího prohlížeče sestav. 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Využití Azure":::

## <a name="licenses-growth-trend"></a>Trend růstu licencí
 
Trend licencí přiřazených všemi zákazníky během vybraného rozsahu dat Osa X představuje měsíce vybraného rozsahu dat a osa Y představuje počet licencí vybraného produktu. Posouváním posuvníku v horní části grafu můžete graf přiblížit ke konkrétnímu časovému období.  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="licence":::

## <a name="next-steps"></a>Další kroky

Další sestavy najdete v tématu [Partnerské centrum Insights.](partner-center-insights.md)
