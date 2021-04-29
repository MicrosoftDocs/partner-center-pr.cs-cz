---
title: Sestavy o prostředcích služby partner Center Insights – CloudAscent
description: Přečtěte si o sestavách PROPER CloudAscent v partnerském centru. Obsahuje informace o prodaných properech zákazníka při nákupu produktů společnosti Microsoft.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 91f64faeec0b97be2797d489e152cb84cbb2e192
ms.sourcegitcommit: 8bd2e2f2f0f6bcd0fa202787df5b3c1f786f88f9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/29/2021
ms.locfileid: "108213434"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>CloudAscent sestavy o prostředcích, které jsou dostupné na řídicím panelu partnerského centra

**Příslušné role**

- Prohlížeč sestav Executive
- Prohlížeč sestav

Řídicí panel partnerského centra poskytuje data o prostředcích ke stažení z programu CloudAscent. Data ukazují pravděpodobnost nákupu produktů společnosti Microsoft pro zákazníky.  Tento článek popisuje rozdělení těchto dat, způsob používání bodování a to, co znamená.

## <a name="summary-definitions"></a>Souhrnné definice

- **Zákazníci** se systémem SMC – Toto je celkový počet zákazníků při stahování proper.  Zákazníci jsou identifikováni partnerem záznamu.
- **Smlouvy s vypršenou platností**– v rámci aktuálního fiskálního roku poskytujeme počet smluv o vypršení platnosti.
- **Otevřené výnosy po vypršení platnosti**– tržby spojené s otevřenými smlouvami o vypršení platnosti.

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Snímek obrazovky se souhrnným řídicím panelem příležitostí pro zákazníky":::

## <a name="cloudascent-smb-segmentation"></a>Segmentace SMB CloudAscent

Segment malý až střední firmy (SMB) je rozdělen na tři samostatné dílčí segmenty.

1. **Hlavní nespravované** zahrnuje největší zákazníky s protokolem SMB s největší příležitostí pro Microsoft. Typický hlavní nespravovaný zákazník sdílí podobné charakteristiky spravovaných účtů, s velkým počtem zaměstnanců, velkým rozpočtům IT a útratou a velkým objemem potenciálních výnosů pro společnost Microsoft.

   V horní části nespravované jsme definovali dva způsoby:

   - **Hlavní nespravovaný uživatel**– obsahuje účty s 300 nebo více zaměstnanci. Účty User-Based jsou skvělé cíle pro první nákup nebo rozšíření produktů pro odběr uživatelů, jako je Microsoft 365, Dynamics 365 nebo Surface.
   - **Založené na hlavních nespravovaných výpočetních** operacích – obsahuje účty s potenciálem Azure větším než $10 000. Účty založené na COMPUTE zahrnují existující Azure. účty s významným potenciálem budoucích let a účty, které ještě ještě kupují Azure, ale mají možnost Azure větší než $10 000.

2. **Středně velké firmy** zahrnují stávající zákazníky a účty nadějných zákazníků s 25 až 300 zaměstnanci.

3. **Malá společnost** zahrnuje firmy s 10-25 zaměstnanci.

4. **Velmi malá společnost** zahrnuje firmy s 1-9 zaměstnanci.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Zákazník podle typu SMC.":::

**Hlavní nespravované** a **střední části podniku** reprezentují vysoké LTV zákazníky pro Microsoft a partnery Microsoftu. Z tohoto důvodu se jedná o oblasti potenciálních zákazníků, které se zaměřují na růst v tomto segmentu. V těchto dvou segmentech jsme lépe umístili k získání soketu s Microsoft 365 monetizovat a D365/Azure obchodními aplikacemi (LOB) a zajistili jsme vysoké LTV pro společnost Microsoft.

Dnes máme dvě klíčové oblasti příležitosti – 1. Náš zákazník přináší růst; odst. i když nám načítáme cloudové sokety s Microsoft 365, máme v Dynamics 365 a Azure velkou příležitost.

Následující snímek obrazovky představuje čtyři segmenty SMB. CloudAscent stanovit prioritu profilace, bodování a modelování všech hlavních nespravovaných a středně velkých obchodních účtů.

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Snímek obrazovky s podsegmenty SMB.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

Protokol SMB používá technologii strojového učení k řízení prodeje a marketingu zákaznických předpovědi v hlavních nespravovaných a středních obchodních segmentech. Jak jsou signály shromažďovány a přeměněny na doporučení týkající se Proper?

- **Shromažďování dat**: webové prohledávací moduly hledají a shromažďují miliardy zákaznických signálů pomocí příkazů k otestování domén společnosti a sledují příspěvky na blogu, stiskněte vydané verze, sociální toky a technická fóra.  Kromě shromážděných signálů se informace o firmographics shromažďují z interních i externích zdrojů, jako je například D&B, interní předplatné Microsoftu a transakční data.

- **Machine Learning**: signály se dopravují do modelu machine learningu, který pro každého zákazníka cloudového produktu a clusteru vytvoří strukturu strukturované datové sady předpovědi pro prodej a marketing.  Každý zákazník se vyhodnotí pomocí podobného modelu jako v horním protokolu SMB od Microsoftu, který určuje přizpůsobení a algoritmy strojového učení, které integrují online chování zákazníka, se definuje jako záměr. Bodování se sloučí do clusterů, které znázorňují prohlédnutí zákazníka k nákupu Microsoft Cloudch produktů.

- **Optimalizace**: systém Machine Learning optimalizuje modely tím, že spotřebovává data transakcí měsíčně a čtvrtletní data předplatného.  Pomocí dat o výher a ztrátách Machine Learning upravuje algoritmy a ověřuje, že modely pracují podle očekávání, tím, že porovnává doporučení clusteru s možnostmi, které se v hlavní části vycházejí.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Snímek obrazovky s protokolem SMB Machine Learning.":::

## <a name="cloudascent-propensity"></a>CloudAscent Proper

Jak se vytvářejí doporučení k properům?

Pomocí signálů shromážděných prostřednictvím webových procházecích a dat z různých zdrojů konsolidujeme firmographics data a sociální signály sociálních médií zákazníka.  Bodování používá tyto signály a data v porovnání modelů pro potřeby a modely bodování pro záměr.

1. Přizpůsobení účtu zákazníka

   - Interní a externí datové body, které definují firmographics.

   - Pro účely bodování se používá model podobného typu, který umožňuje porovnat zákazníky a zjistit, jestli jsou potenciálně vyhovující Microsoft Cloud produktů.

   - Podle skóre se aktualizuje čtvrtletní

2. Záměr účtu zákazníka

   - Signály týkající se sociálních médií a definování záměrů online zákazníka.

   - Bodování záměru je překrytí na základě přizpůsobení, aby bylo možné definovat clustery.

   - Bodování záměru se aktualizuje měsíčně.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscenté prediktivní modely protokolu SMB.":::

3. Clustering

   Signály pro přizpůsobení a záměr jsou konsolidovány do skóre clusteringu. CloudAscent má čtyři clustery:

      - Zákazníci, kteří jsou nyní připravení k prodeji
      - Vyhodnocení – zákazníci připravení pro marketing
      - Nurture – kampaně pro osvětu
      - Vzdělávání – vzdělávání a monitorování pro záměr

   Clustering umožňuje uživatelům zaměřit se na konkrétní zákazníky na prodejní a marketingové iniciativy na základě faktorů segmentů, například: produkt, geografické prostředí, odvětví a vertikální.

   Karta **model PROPER** v sešitech CloudAscent sdílí PROPER a odhadované tržby za prázdných znaků. Pokud chcete definovat clustery, které je vhodné a záměr, Projděte si následující kroky:

      1. Pomocí modelů ML si předem vypočítáme skóre a skóre záměru zákazníka na škále 100.  Přesné výsledky se budou lišit v závislosti na modelů ML.  Příklad skóre níže:

         |**Klasifikace**|**Podtržítk**|
         |---------|:---------|
         |Vysoká|75 – 100|
         |Střední|55 – 74|
         |Nízká|30 - 54|
         |Velmi nízké|0 - 29|

      2. Pomocí výše uvedeného pravidla klasifikujeme společnosti tak, aby byly vysoké, střední, nízké a velmi nízké v rámci přizpůsobení a signálů pro zákazníky.

      3. Na 2D matrici vykreslíme vydaných a vystupujících signálů zákazníků s každým průnikem, který představuje proper. Například vysoká velikost + vysoká záměr = a1, který představuje nejvyšší proper.

      4. Nakonec tyto segmenty seskupují clustery.  Například, a1, a2, a3, A4 tvoří cluster Act Now.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent modely.":::

   Pro tyto zákazníky doporučujeme cílit na Act nyní a vyhodnocovat zákazníky.

## <a name="cloudascent-products--models"></a>CloudAscent produkty & modely

Následující obrázek poskytuje zobrazení jednotlivých modelů PROPER v rámci CloudAscent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent model proper.":::

Prázdné modely se skládají z předpovědi pro stávající zákazníky Microsoftu, kde nemají produkt a/nebo jsou noví zákazníci, kteří používají zákazníky v rámci zákazníků.

Modely přeprodat používají data transakcí k předpovídání potenciálu přeprodat v Azure a Microsoft 365 SKU.

Tito zákazníci už budou mít Azure i Microsoft 365 a model přeprodat ukazuje, že si pravděpodobně koupí více svých stávajících SKU.

EOS sdílí zákazníky služby EOS (End of Service) pro Win 7, Office 2010, SQL Server a Windows Server. Data EOS se předají z prodeje MS a překrývají se pomocí modelování PROPER CloudAscent, kde jsou k dispozici. EOS data v moderní práci a prodej v Azure.
