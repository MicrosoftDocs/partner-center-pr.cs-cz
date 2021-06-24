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
ms.openlocfilehash: cca136670fa2891eea32e4561b97692ca98a77a9
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565402"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>Přehled sestav řídicích panelů dostupných ve službě partner Center – přehledy
 
**Příslušné role**: globální správce | Agent správce | Prohlížeč sestav | Prohlížeč sestav Executive

Řídicí panel přehled Insights nabízí zobrazení snímků klíčových ukazatelů výkonu (KPI), jako jsou zákazníci, předplatná, výnosy za využití Azure a licence. V sestavě přehledu můžete vizualizovat následující grafy.

- Souhrn  
- Geografické rozšiřování vašich zákazníků, předplatných a licencí  
- Trend růstu pro zákazníky 
- Geometrický trend předplatných 
- Trend růstu spotřebovaných výnosů v Azure 
- Trend růstu licencí 

## <a name="summary"></a>Souhrn

Souhrn obsahuje informace o zákaznících, výnosech spotřebovaných v Azure (ACR), prodávaných předplatných, aktivních předplatných a licencích. 

:::image type="content" source="images/pci/summary.png" alt-text="Souhrnné licence.":::

Další informace o jednotlivých částech souhrnu najdete v tématu.

### <a name="customers"></a>Zákazníci

Oblast **zákazníci** zahrnuje:

- Aktuální počet všech zákazníků s alespoň jedním aktivním předplatným přidruženým k vaší firmě prostřednictvím různých typů přiřazení a všech cloudových produktů.
- Procentuální nárůst počtu zákazníků v průběhu vybraného období.
- Mikrograf prezentuje trend počtu zákazníků v měsíci v rámci vybraného rozsahu kalendářních dat.

### <a name="azure-consumed-revenue-acr"></a>Tržby spotřebované za Azure (ACR)

Oblast **Azure spotřebované tržby (ACR)** na souhrnu zahrnuje:

- Celkový počet ACR (v amerických dolarech) přidaných na vybraný rozsah dat
- Procentuální nárůst nebo pokles v ACR s atributy (v amerických dolarech) v průběhu vybraného období.
- Mikrograf prezentuje měsíční trend ACR v amerických dolarech, na které jste ve vybraném rozsahu kalendářních dat. 

> [!NOTE]
> ACR data jsou k dispozici uživatelům, kterým byla přiřazena role vedoucího prohlížeče sestav.
 
### <a name="subscriptions-sold"></a>Prodávaná předplatná

Vydaná oblast **předplatných** obsahuje tyto informace:

- Celkový aktuální počet předplatných cloudových produktů (aktivních a neaktivních) prodaných nebo spravovaných vámi.  
- Procentuální nárůst nebo pokles předplatných během vybraného rozsahu kalendářních dat.
- Mikrograf prezentuje trend celkového počtu předplatných v rámci vybraného rozsahu dat v měsíci.

### <a name="active-subscriptions"></a>Aktivní předplatná

Oblast **aktivních předplatných** na souhrnu zahrnuje:

- Aktuální počet odběrů cloudových produktů s aktivním využitím měřený na základě telemetrie produktů. Vyloučí se všechna zkušební předplatná Azure.  
- Procentuální nárůst aktivních předplatných v rámci vybraného rozsahu kalendářních dat.
- Mikrograf prezentuje trend aktivních předplatných za měsíc v průběhu vybraného období.
 
### <a name="licenses-deployed"></a>Nasazené licence

Oblast **nasazených licencí** zahrnuje tyto informace:
 
- Počet všech licencí cloudových produktů nasazených ve vašich zákaznických předplatných za vybrané časové období. 
- Procentuální nárůst nebo pokles těchto licencí v průběhu vybraného rozsahu dat. 
- Mikrograf znázorňuje trend měsíčního měsíčního počtu přiřazených licencí v rámci vybraného rozsahu dat.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Geografické rozšiřování vašich zákazníků, předplatných a licencí

Toto zobrazení je geografickou distribucí celkových zákazníků, předplatných a licencí podle země zákazníka. Výběrem různých karet zobrazíte všechny tyto přehledy na mapě. Můžete vyhledat a vybrat zemi v mřížce pro přiblížení do umístění v mapě. Kliknutím na tlačítko domů na mapě se vraťte k původnímu zobrazení. Po kliknutí na jednotlivé karty (například zákazníci, předplatná) se zobrazí hodnota metriky pro každou zemi a procento celku pro danou zemi.  

:::image type="content" source="images/pci/geosummary.png" alt-text="Zeměpisné Shrnutí":::

## <a name="customers-growth-trend"></a>Trend růstu pro zákazníky

Pro vybraný rozsah dat se počítá měsíční trend z celkového počtu zákazníků. Osa X představuje měsíce vybraného rozsahu kalendářních dat a osa Y představuje celkový počet zákazníků pro daný měsíc. 

:::image type="content" source="images/pci/customergrowth.png" alt-text="růst trendů pro zákazníky.":::

## <a name="subscriptions-growth-trend"></a>Geometrický trend předplatných

To indikuje trend počtu předplatných zákazníků pro vybraný rozsah kalendářních dat. Osa X představuje měsíce vybraného rozsahu kalendářních dat a osa Y představuje počet předplatných vybraných pro daný produkt. Posuňte se přes posuvník nad grafem, aby se graf zvětšil na konkrétní časové období. 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="Trend růstu předplatného.":::

## <a name="azure-consumed-revenue-growth-trend"></a>Trend růstu spotřebovaných výnosů v Azure

Měsíční trend spotřebovaných výnosů v Azure v amerických dolarech, který se na vás přiřadí za vybraný rozsah kalendářních dat. Osa X představuje měsíce vybraného rozsahu kalendářních dat a osa Y představuje celkový počet spotřebovaných výnosů za měsíc v amerických dolarech.

> [!NOTE]
> ACR budou viditelné pouze uživatelům, kterým byla přiřazena role vedoucího prohlížeče sestav. 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Využití Azure.":::

## <a name="licenses-growth-trend"></a>Trend růstu licencí
 
Trend licencí přidaných všemi zákazníky během vybraného rozsahu kalendářních dat. Osa X představuje měsíce vybraného rozsahu kalendářních dat a osu Y představuje počet licencí vybraného produktu. Posuňte se přes posuvník nad grafem, aby se graf zvětšil na konkrétní časové období.  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="vázaný.":::

## <a name="next-steps"></a>Další kroky

Další sestavy najdete v tématu [Přehled služby partner Center](partner-center-insights.md).
