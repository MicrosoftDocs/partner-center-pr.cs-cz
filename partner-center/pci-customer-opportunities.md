---
title: Partnerské centrum Insights – sestavy sklonu CloudAscent
description: Seznamte se se zprávami CloudAscent Propensity v Partnerské centrum. Obsahuje informace o náchylnosti zákazníka k nákupu produktů Microsoftu.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153034"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Sestavy CloudAscent Propensity dostupné na Partnerské centrum řídicím panelu

**Odpovídající role:** Prohlížeč sestav executive | Prohlížeč sestav

Řídicí Partnerské centrum poskytuje data o sklonu ke stažení z programu CloudAscent. Data ukazují pravděpodobnost, že zákazníci budou kupovat produkty Microsoftu.  Tento článek popisuje rozpis těchto dat, způsob použití vyhodnocování a co to znamená.

## <a name="summary-definitions"></a>Souhrnné definice

- **Zákazníci SMC**– Celkový počet zákazníků, kteří se ke stažení s náchylností stahují.  Zákazníci jsou identifikováni partnerem záznamu.
- **Vypršení platnosti** smluv – v rámci aktuálního fiskálního roku zadáte počet smluv, u které vyprší platnost.
- **Open Expiring Revenue**–Výnosy spojené se smlouvami o otevření, u které vyprší platnost.

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Snímek obrazovky s řídicím panelem Souhrn příležitostí zákazníků":::

## <a name="cloudascent-smb-segmentation"></a>Segmentace SMB v CloudAscent

Segment SMB (Small to Medium Business) je rozdělen do tří různých dílčích segmentů.

1. **Top Unmanaged zahrnuje** největší zákazníky SMB s největší příležitostí pro Microsoft. Typickí nespravované zákazníky mají podobné vlastnosti jako spravované účty s velkým počtem zaměstnanců, velkými rozpočty a výdaje na IT a velkými objemy potenciálních výnosů pro Microsoft.

   Nespravované prostředky definujeme dvěma způsoby:

   - **Top Unmanaged User Based –zahrnuje** účty se 300 nebo více zaměstnanci. Účty User-Based jsou skvělé cíle pro první nákup nebo rozšíření produktů pro odběr uživatelů, jako je Microsoft 365, Dynamics 365 nebo Surface.
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

- **Shromažďování dat:** Webové prohledávací systémy prohledávače skenují a shromažďují miliardy signálů zákazníků příkazem ping na domény společnosti a monitorují blogové příspěvky, tiskové zprávy, sociální streamy a technická fóra.  Kromě shromážděných signálů se firemní údaje shromažďují z interních i externích zdrojů, jako jsou D&B, interní předplatné Microsoftu a transakční data.

- **Machine Learning:** Signály se předá do modelu strojového učení, který každému zákazníkovi předpovídá strukturovaná datová sada předpovědí prodeje a marketingu podle cloudových produktů a shluků.  Každý zákazník má skóre s použitím podobného modelu pro nejlepší SMB Microsoftu, který určuje algoritmy Fit zákazníka a strojové učení, které integrují online chování zákazníka, které definují záměr. Bodování se sloučí do clusterů, které ukazují náchylnost zákazníka k nákupu cloudových produktů Microsoftu.

- **Optimalizace:** systém Machine Learning optimalizuje modely tím, že každý měsíc spotřebovává data transakcí a čtvrtletně data předplatného.  Pomocí dat o výhře/ztrátě Machine Learning upraví algoritmy a ověří, že modely fungují podle očekávání, porovnáním doporučení clusteru s příležitostmi v MSX.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Snímek obrazovky se strojového učením SMB":::

## <a name="cloudascent-propensity"></a>CloudAscent Propensity

Jak se vytvářejí doporučení pro sklony?

Pomocí signálů shromážděných prostřednictvím webových prohledávacích systémů a dat poskytovaných z různých zdrojů konsolidujeme firemní data a signály zákazníků ze sociálních sítí.  Bodování používá tyto signály a data v modelech porovnání pro fitovací a bodovací modely záměru.

1. Přizpůsobení zákaznického účtu

   - Interní a externí datové body, které definují pevné údaje.

   - Bodování fitů používá pro náš nejlepší protokol SMB podobný model, který porovnává zákazníky a zkoumá, jestli se hodí pro cloudové produkty Microsoftu.

   - Vyhodnocování fitů se aktualizuje čtvrtletně.

2. Záměr účtu zákazníka

   - Signály související se sociálních sítěmi a online chováním zákazníka definují záměr.

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

         |**Classification**|**Podtržítk**|
         |---------|:---------|
         |Vysoká|75 – 100|
         |Střední|55 – 74|
         |Nízká|30 - 54|
         |Velmi nízké|0 - 29|

      2. Pomocí výše uvedeného pravidla klasifikujeme společnosti tak, aby byly vysoké, střední, nízké a velmi nízké napříč signály Customer Fit i Intent Signals.

      3. Vykreslujeme signály zákazníka fit a záměr na 2D matici, kde každý průnik představuje sklon. Příklad: High Fit + High Intent = A1 představující nejvyšší sklon.

      4. Nakonec se tyto segmenty seskupí do shluků.  Například cluster Act Now tvoří A1, A2, A3 a A4.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Modely CloudAscent.":::

   Pro tyto zákazníky doporučujeme zacílení na Jednat hned a Vyhodnotit zákazníky.

## <a name="cloudascent-products--models"></a>CloudAscent Products & Models

Následující obrázek poskytuje zobrazení jednotlivých modelů sklonů v CloudAscent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent propensity model.":::

Prázdné modely se skládají z předpovědí pro stávající zákazníky Microsoftu, kteří nemají produkt nebo jsou novými potenciálními zákazníky.

Modely upsell používají transakční data k předpovídání potenciálního prodávat v Azure a Microsoft 365 skladových náklady.

Tito zákazníci už budou mít Azure nebo Microsoft 365 a model pro prodej ukazuje, že si pravděpodobně koupí větší část své stávající SKU.

EOS sdílí zákazníky s EOS (End of Service) pro Win 7, Office 2010, SQL Server a Windows Server. Data EOS se načtou z MS Sales a přelásní se modelováním sklonu CloudAscent, pokud je k dispozici. Data eOS se nachází v roli Moderní práce a Azure Sales.
