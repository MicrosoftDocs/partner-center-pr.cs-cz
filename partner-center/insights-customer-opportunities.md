---
title: Partnerské centrum Přehledy – Sestavy sklonů CloudAscent
description: Seznamte se se zprávami CloudAscent Propensity v Partnerské centrum. Obsahuje informace o náchylnosti zákazníka k nákupu produktů Microsoftu.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 6916d44e3f028fbfd788d3bee54671dbadd874d1
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376582"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Sestavy CloudAscent Propensity dostupné na Partnerské centrum řídicím panelu

**Vhodné role:** Prohlížeč sestav executive | Prohlížeč sestav

Řídicí Partnerské centrum poskytuje data o sklonech ke stažení z programu CloudAscent. Data ukazují pravděpodobnost, že zákazníci budou kupovat produkty Microsoftu.  Tento článek popisuje rozpis těchto dat, způsob použití vyhodnocování a co to znamená.

## <a name="summary-definitions"></a>Souhrnné definice

- **Zákazníci SMC**– Celkový počet zákazníků, kteří se ke stažení s náchylností stahují.  Zákazníci jsou identifikováni partnerem záznamu.
- **Vypršení platnosti** smluv – V rámci aktuálního fiskálního roku zadáte počet smluv, u které vyprší platnost.
- **Open Expiring Revenue**–Výnosy spojené se smlouvami o otevření, u které vyprší platnost.

:::image type="content" source="images/insights/customer-opportunity-1.png" alt-text="Snímek obrazovky s řídicím panelem Souhrn příležitostí zákazníků":::

## <a name="cloudascent-smb-segmentation"></a>Segmentace SMB v CloudAscent

Segment SMB (Small to Medium Business) je rozdělen do tří různých dílčích segmentů.

1. **Nejspravovaná služba** zahrnuje největší zákazníky SMB s největší příležitostí pro Microsoft. Typickí nespravované zákazníky mají podobné vlastnosti jako spravované účty s velkým počtem zaměstnanců, velkými rozpočty a výdaje na IT a velkými objemy potenciálních výnosů pro Microsoft.

   Nespravované prostředky definujeme dvěma způsoby:

   - **Top Unmanaged User Based –zahrnuje** účty se 300 nebo více zaměstnanci. User-Based účty jsou skvělými cíli pro první nákup nebo rozšíření uživatelských produktů předplatného, jako jsou Microsoft 365, Dynamics 365 nebo Surface.
   - **Top Unmanaged Compute Based** (Nejspravovanější výpočetní prostředky) – zahrnuje účty s Potenciálním azure vyšším než 10 000 USD. Mezi výpočetní účty patří existující Azure. účty s významnými možnostmi z budoucího roku a účty, které ještě nemají možnost zakoupit Azure, ale mají potenciál pro Azure větší než 10 tisíc USD.

2. **Medium Business** zahrnuje stávající zákazníky a potenciální zákazníky s 25 až 300 zaměstnanci.

3. **Small Business** zahrnuje firmy s 10 až 25 zaměstnanci.

4. **Velmi malá firma zahrnuje** firmy s 1–9 zaměstnanci.

:::image type="content" source="images/insights/customer-opportunity-2.png" alt-text="Zákazník podle typu SMC":::

**Nejspravovaná** a **střední** obchodní dílčí období představují zákazníky s vysokou životností (LTV) pro Microsoft a partnery Microsoftu. Z tohoto důvodu jsou hlavní oblastí zaměření na řízení růstu v tomto segmentu. V těchto dvou dílčích návěscích máme lepší pozici k získání soketu s Microsoft 365, dalšímu monetizaci pomocí obchodních aplikací D365/Azure a realizaci vysoké LTV pro Microsoft.

Dnes máme dvě klíčové oblasti příležitostí – 1. náš zákazník zvyšuje růst. 2. I když si vedeme dobře se získáním cloudových soketů vedoucích Microsoft 365, máme v Dynamics 365 a Azure velkou příležitost.

Následující snímek obrazovky představuje čtyři dílčí aplikace SMB. CloudAscent upřednostňuje profilaci, bodování a modelování všech nejspravovaných a středních obchodních účtů.

:::image type="content" source="images/insights/customer-opportunity-3.png" alt-text="Snímek obrazovky s dílčími aplikacemi SMB":::

## <a name="cloudascent-machine-learning"></a>CloudAscent – Machine Learning

SMB využívá technologii strojového učení k řízení prodejních a marketingových předpovědí zákazníků v segmentech Top Unmanaged a Medium Business. Jak se signály shromažďují a převedou na doporučení ke záměně?

- **Shromažďování dat:** Webové prohledávací systémy prohledávače skenují a shromažďují miliardy signálů zákazníků příkazem ping na domény společnosti a monitorují blogové příspěvky, tiskové zprávy, sociální streamy a technická fóra.  Kromě shromážděných signálů se firemní údaje shromažďují z interních i externích zdrojů, jako jsou D&B, interní předplatné Microsoftu a transakční data.

- **Machine Learning:** Signály se předá do modelu strojového učení, který každému zákazníkovi předpovídá strukturovaná datová sada předpovědí prodeje a marketingu podle cloudových produktů a shluků.  Každý zákazník má skóre s použitím podobného modelu pro nejlepší SMB Microsoftu, který určuje algoritmy Fit zákazníka a algoritmy strojového učení, které integrují online chování zákazníka, které definují jako záměr. Bodování se sloučí do clusterů, které ukazují sklon zákazníka k nákupu cloudových produktů Microsoftu.

- **Optimalizace:** systém Machine Learning optimalizuje modely tím, že každý měsíc spotřebovává data transakcí a čtvrtletně data předplatného.  Pomocí dat o výhře/ztrátě Machine Learning upraví algoritmy a ověří, že modely fungují podle očekávání, porovnáním doporučení clusteru s příležitostmi, na které se v MSX pracovalo.

:::image type="content" source="images/insights/customer-opportunity-4.png" alt-text="Snímek obrazovky se strojového učením SMB":::

## <a name="cloudascent-propensity"></a>CloudAscent Propensity

Jak se vytvářejí doporučení k náchylnosti?

Pomocí signálů shromážděných prostřednictvím webových prohledávacích systémů a dat poskytovaných z různých zdrojů konsolidujeme firemní data a signály zákazníků ze sociálních sítí.  Bodování používá tyto signály a data v modelech porovnání pro fitovací a bodovací modely záměru.

1. Přizpůsobení zákaznického účtu

   - Interní a externí datové body, které definují pevné údaje.

   - Bodování fitů používá pro náš nejlepší protokol SMB podobný model, který porovnává zákazníky a zkoumá, jestli se hodí pro cloudové produkty Microsoftu.

   - Vyhodnocování fitů se aktualizuje čtvrtletně.

2. Záměr účtu zákazníka

   - Signály související se sociálních sítěmi a online chováním zákazníka definují záměr.

   - Bodování záměru je nadvrchu vhodné k definování shluků.

   - Bodování záměru se aktualizuje každý měsíc.

   :::image type="content" source="images/insights/customer-opportunity-5.png" alt-text="CloudAscent SMB predictive models.":::

3. Clustering

   Signály pro fit a záměr se konsolidují do skóre shlukování. CloudAscent má čtyři clustery:

      - Jednat hned – zákazníci připravení na prodej
      - Vyhodnocení – zákazníci připravení na marketing
      - Rozvoj – zvyšování povědomí o kampaních
      - Vzdělávání – vzdělávání a monitorování záměru

   Clustering umožňuje uživatelům cílit konkrétní zákazníky na prodejní a marketingové iniciativy založené na faktorech segmentů, například na produkt, geografické oblasti, odvětví a vertikálně.

   Karta **Model sklonů v** CloudAscent Workbooks sdílí sklon a odhadované výnosy z prázdných znaky. Při definování clusteringu fitu a záměru provedeme následující kroky:

      1. Pomocí ML modelů nejprve vypočítáme skóre fitu zákazníka a skóre záměru na škále 100.  Přesné skóre se bude lišit v závislosti na ML modelech.  Příklady skóre níže:

         |**Classification**|**Skóre**|
         |---------|:---------|
         |Vysoká|75 - 100|
         |Střední|55 - 74|
         |Nízká|30 - 54|
         |Velmi nízká|0 - 29|

      2. Pomocí výše uvedeného pravidla klasifikujeme společnosti tak, aby byly vysoké, střední, nízké a velmi nízké napříč signály Customer Fit i Intent Signals.

      3. Vykreslujeme signály zákazníka fit a záměr na 2D matici s každým průnikem, který představuje sklon. Příklad: High Fit + High Intent = A1, který představuje nejvyšší sklon.

      4. Nakonec se tyto segmenty seskupí do shluků.  Například A1, A2, A3, A4 tvoří cluster Act Now.

         :::image type="content" source="images/insights/customer-opportunity-6.png" alt-text="Modely CloudAscent.":::

   Pro tyto zákazníky doporučujeme zacílení na Jednat hned a Vyhodnotit zákazníky.

## <a name="cloudascent-products--models"></a>CloudAscent Products & Models

Následující obrázek poskytuje zobrazení jednotlivých modelů sklonů v rámci CloudAscent:

:::image type="content" source="images/insights/customer-opportunity-7.png" alt-text="CloudAscent propensity model.":::

Prázdné modely se skládají z předpovědí pro stávající zákazníky Microsoftu, kteří nemají produkt nebo jsou novými potenciálními zákazníky.

Modely upsell používají transakční data k předpovídání potenciálního prodávat v Azure a Microsoft 365 skladových náklady.

Tito zákazníci už budou mít Azure nebo Microsoft 365 a model pro prodej ukazuje, že si pravděpodobně koupí větší část své stávající SKU.

EOS sdílí zákazníky s EOS (End of Service) pro Win 7, Office 2010, SQL Server a Windows Server. Data EOS se načtou z MS Sales a přetahuje se modelováním sklonu CloudAscent, pokud je k dispozici. Data eOS se nachází v oblasti moderní práce a azure sales.
