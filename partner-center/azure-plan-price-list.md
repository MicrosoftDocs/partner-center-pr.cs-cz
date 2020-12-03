---
title: Ceník plánu Azure pro partnery CSP
ms.topic: how-to
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak můžou partneři programu CSP používat Partnerské centrum k zobrazení ceníku pro předplatná v rámci plánu Azure.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 02cea980626ec32d3dd60f646b1f8744130792ea
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534722"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Ceník nového obchodního prostředí v CSP pro Azure

**Příslušné role**

- Agent správce
- Správce fakturace
- Globální správce
- Agent helpdesku
- Agent prodeje
- Správce správy uživatelů

Ceník pro nové prostředí Azure Commerce v CSP je zveřejněný v partnerském centru. Ceník se dynamicky doručuje do správného souboru v reálném čase a ceny se zobrazují jenom v USD. Fakturace se ale provádí v podporované měně, která se vztahuje na umístění měny zákazníka. Další informace o fakturaci v umístění měny zákazníka najdete v tématu [plán Azure – fakturace](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Podívejte se na ceny předplatných podle plánu Azure

1. V nabídce partnerského centra na levé straně vyberte **prodávat** a pak vyberte **Marketplace**.

2. V části ceny plánu Azure vyberte zemi, pro kterou chcete počítat s cenami.

3. Vedle **pole typ exportu** vyberte **ceny za využití plánu Azure**, **ceny za rezervace plánu Azure** nebo **devizové sazby**. 

>[!NOTE] 
>**Sazby za FX** nejsou specifické pro země.

4. V poli **ceny pro datum** vyberte datum, které chcete, například **aktuální**.

   :::image type="content" source="images/azure/pricingnew.png" alt-text="konkrétní země":::

>[!NOTE] 
>Můžete exportovat dva různé ceníky – ceny plánu Azure a ceny třetích stran na webu Marketplace.

## <a name="azure-price-list-specifics"></a>Specifické ceny Azure pro ceník

- Ceny plánu Azure budou k dispozici na stránce Marketplace v partnerském centru v části **prodej**.

- K dispozici jsou exporty pro služby spotřeby plánů Azure, Azure Reservations a míry FX.

- Mezi možnosti exportu patří:

  - **Dnešní ceny**: zahrnuje všechny měřiče a ceny od 1. měsíce k aktuálnímu datu aktuálního měsíce. To zahrnuje nové ceny, změněné ceny nebo odebrané ceny. Všechny ceny budou mít počáteční počáteční a koncové datum, které vysvětlí, jestli jsou nové nebo odebrané.

  - **Ceny za předchozí měsíc**: stažení každého typu prostředku bude po měsících. Pro soubory s cenami budou zahrnuty všechny měřiče, které byly během daného měsíce k dispozici. Pokud se v průběhu měsíce objevilo nové měření, zobrazí se mi jako měřič s datem účinnosti, který odráží jeho dostupnost. Podobně jako u cen, které jsou vyřazeny, zobrazuje s nejefektivnějším koncovým datem, které popisují, kdy již nejsou k dispozici.

  - **Frekvence FX**: pro stažení za den před 1.18:00 PST budou k dispozici poplatky za FX. Například pokud chcete, aby se sazby za listopad, stáhly do 31. října. Sazby za předchozí měsíc budou také k dispozici.

- Ceny v ceníkech jsou přímé ceny. Někteří partneři můžou mít nárok na kredity, které získali partneři. Informace o tom, jak se vypočítal partner získaný kredit, najdete v tématu [Výpočet a platby pro partnerský účet](partner-earned-credit-explanation.md).

- **Opravňující služby**: získaný partnerský kredit se vztahuje na služby uvedené v **cenovém** partnerovi pro Azure Plan – ceny se můžou exportovat na stránce s [cenami plánu Azure](https://partner.microsoft.com/commerce/sales) . Všimněte si, že existují výjimky, včetně produktů třetích stran, které jsou označené jako "třetí strana" ve sloupci značky v seznamu cena za využití plánu Azure a rezervacích plánu Azure.

## <a name="price-list-data"></a>Data ceníku

|**Pole**   |**Popis**   |
|--------------------------|:---------------------------|
|ProductTitle  |Název nebo název produktu|
|ProductID   |ID produktu|
|SKuId|ID SKU|
|SkuTitle|Název nebo název SKU|
|Publisher|1. strana bude vždycky Microsoft|
|SkuDescription|Popis SKU|
|UnitOfMeasure|Jednotky, které se účtují nebo účtují|
|TermDuration|U produktů založených na termínech se délka podmínky vztahuje na rezervace.|
|Uvádět|Uvedení ceny na trh|
|Měna|Měna cen|
|Jednotková cena|Cena za jednotku|
|PricingTierRangeMin|Pro vrstvené ceny platí minimální cena.|
|PricingTierRangeMax|Pro vrstvené ceny platí maximální cena.|
|EffectiveStartDate|Počáteční datum cen|
|EffectiveEndDate|Koncové datum cen|
|MeterId|ID měřiče SKU produktu|
|MeterType|Typ měřiče|
|Značky|Vlastnosti položky, pro ceny plánu Azure se bude jednat o Azure nebo Azure a rezervace (pro konkrétně rezervace).|

Ceníky pro plán Azure můžete exportovat ze [stránky ceny a nabídky](https://partner.microsoft.com/dashboard/sell/pricingandoffers) v partnerském centru.

## <a name="tiered-pricing"></a>Vrstvené ceny

Některé služby spotřeby plánu Azure podporují vrstvené ceny. Partneři můžou tyto produkty a SKU najít v ceníku plánu Azure. Položky, které mají hodnoty ve sloupcích rozsah cenové úrovně, umožňují partnerům pochopit cenu na základě využití. V níže uvedeném příkladu máte k dispozici jednu skladovou položku produktu se třemi cenovými úrovněmi.

|**ProductId**   |**SkuId**   |**Jednotková cena**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|.50|100001|9223372036854780000|
|DDD123456ABC|01AB|.80|101|100000|
|DDD123456ABC|01AB|1|1|100|

Pokud se v tomto příkladu používají jednotky 101, účtuje se cena 100,80. Prvních 100 jednotek je jedna a další jednotka se účtuje za. 80.

## <a name="pricing-api-for-azure-plan"></a>Cenové rozhraní API pro plán Azure

Pomocí [cenového rozhraní API](/partner/develop/pricing) můžete načíst ceny plánu Azure pro spotřebu a rezervace prostřednictvím kódu programu. Můžete také získat cizí kursy.

Cenové rozhraní API se nachází v jiném koncovém bodě než ostatní rozhraní API partnerského centra. Informace o cenách zahrnují ceny za měřiče v USD pro plánování prostředků Azure a ceny za rezervace, které se vztahují na předplatné plánu Azure.

Toto rozhraní API také umožňuje partnerům načítat měsíční sazby, protože ceny plánu Azure jsou jenom v USD. Rozhraní API můžete použít k načtení cen i devizových sazeb pro aktuální měsíc nebo předchozí měsíce.

>[!NOTE]
> Cenové rozhraní API je specifické pro ceny plánu Azure. Pořád byste měli používat stávající RateCard API a ceníky publikované na stránce ceny a nabídky partnerského centra pro prostředky Azure nebo rezervace nasazené do předplatných plánů mimo Azure. Cenové rozhraní API pro Azure Plan nepodporuje software, Marketplace ani ceny založené na licencích, jako je Microsoft 365 nebo Dynamics 365.

Další informace o cenách plánu Azure a rozhraní API pro cizí kurz najdete v [dokumentaci k rozhraní API](/partner/develop/pricing)pro celou cenu.

## <a name="next-steps"></a>Další kroky

- [Správa předplatných a prostředků v rámci plánu Azure](azure-plan-manage.md)