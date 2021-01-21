---
title: Řídicí panel sestavy stažení přehledů
ms.topic: article
ms.date: 10/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se stahovat a exportovat data z jednotného řídicího panelu pro vytváření sestav partnerského centra a ze sestav služby partner Center Insights.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c7b0be301b9c0fc56200c128b225fc849a2f04c2
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/19/2020
ms.locfileid: "92527769"
---
# <a name="download-reports"></a>Stažení sestav

**Příslušné role**
- Prohlížeč sestav Executive
- Prohlížeč sestav

## <a name="introduction"></a>Úvod

Centrum sestav stáhnout na řídicím panelu přehledy umožňuje exportovat nezpracované sady dat, které vystavují sestavy služby partner Center Insights ve formátu TSV (hodnoty oddělené tabulátory). To vám umožní podrobnější analýzu dat na základě obchodních potřeb.

Po vygenerování bude sestava k dispozici v části **vygenerované sestavy** , kde můžete stáhnout a analyzovat pomocí nástrojů, jako je Microsoft Excel.

**Vytvořit novou sestavu**

Pokud chcete vygenerovat sestavu, nejdřív ji vyberte v rozevíracím seznamu **Vybrat sestavu** . Pak v rozevíracím seznamu **Vybrat rozsah dat** vyberte rozsah kalendářních dat. Vyberte **Generovat**. Sestava bude vygenerována ve formátu hodnot oddělených tabulátory (TSV) a bude k dispozici ke stažení v části **generované sestavy** během několika minut. Sestavy vygenerované během předchozích 14 dnů budou k dispozici ke stažení.

:::image type="content" source="images/pci/create-new-report.png" alt-text="Vytvořit novou sestavu":::

:::image type="content" source="images/pci/generated-reports.png" alt-text="Vygenerované sestavy":::

>[!NOTE] 
>Sestavy mohou stahovat pouze uživatelé, kteří jsou správci sestav od vedoucího. Další informace o přístupu na základě rolí k sestavám řídicího panelu Insights najdete v tématu [role PCI](pci-roles.md). 

## <a name="available-reports"></a>Dostupné sestavy

Ke stažení jsou k dispozici následující sestavy:

**Partnerský profil** poskytuje podrobnosti související s partnerem. V sestavě jsou k dispozici podrobnosti, jako je ID partnera, jméno partnera, město partnera, partnerská země atd. Pro tuto sestavu se nepoužijí žádné agregace ani lookback.

**Podrobnosti o zákaznících** poskytují informace o zákaznících, ke kterým je přidružen partner. Poskytuje také klíčové metriky, jako jsou prodávané licence, agregované ACR a tak dále. Sestava se agreguje měsíčně.

**Podrobnosti o předplatných** poskytují podrobné informace o předplatných, která jsou prodávaná nebo spravovaná partnerem, spolu s informacemi o zákaznících. Sestava se agreguje měsíčně.

**Využití Azure** poskytuje podrobné informace o využití Azure. Tyto podrobnosti jsou pro předplatná Azure prodávaná nebo spravovaná partnerem. Podrobnosti o využití jsou rozděleny podle kategorie měřiče a dalších klíčových dimenzí. Sestava se agreguje měsíčně.

**Office 365 – použití licencí** poskytuje podrobnosti o využití licencí O365 prodávaných nebo spravovaných partnerem. Poskytuje taky informace o zákaznících a klíčová metriky, jako jsou aktivní uživatelé (MAU), kvalifikované nároky atd. Sestava se agreguje měsíčně.

**Enterprise mobility – využití licencí**  poskytuje podrobnosti o využití licencí Enterprise mobility vydaných nebo spravovaných partnerem. Poskytuje taky informace o zákaznících a klíčová metriky, jako jsou aktivní uživatelé (MAU), kvalifikované nároky atd. Sestava se agreguje měsíčně.

**Dynamics 365 – použití licencí** poskytuje podrobnosti o využití licencí D365 vydaných nebo spravovaných partnerem. Poskytuje taky informace o zákaznících a klíčová metriky, jako jsou aktivní uživatelé (MAU), kvalifikované nároky atd. Sestava se agreguje měsíčně.

**Power BI – použití licencí** poskytuje podrobné informace o využití licencí Power BI vydaných nebo spravovaných partnerem. Poskytuje taky informace o zákaznících a klíčová metriky, jako jsou aktivní uživatelé (MAU), kvalifikované nároky atd. Sestava se agreguje měsíčně.

**Školení** poskytují podrobné informace, jako jsou zkoušky, certifikace, posouzení, běhy, kurzy, které dokončili nebo provedou zaměstnanci partnera.

**Microsoft Learn** poskytuje podrobnosti o modulech, podrobnostech o dokončeních studijních cest spolu s podrobnostmi o uživateli pro partnera.

**Kompetence – souhrn a historie** poskytují podrobné informace o všech kompetencích, které jsou buď aktivní, probíhající nebo v ohrožení tohoto partnera. Zahrnuje také historii všech kompetencí dosažených partnerem.

**Kompetence – podrobnosti o výkonu** poskytují podrobné informace o tom, jak partner pracuje s ohledem na klíčové ukazatele výkonu pro dosažení určité sady kompetencí.

