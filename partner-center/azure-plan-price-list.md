---
title: Ceník plánu Azure pro partnery CSP
ms.topic: how-to
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak zprostředkovatelé programu CSP Partnerské centrum k zobrazení ceníku předplatných v rámci plánu Azure.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 6d8e73e664d400e8e6d80e529326e566c5fd88a8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149566"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Ceník nového obchodního prostředí v CSP pro Azure

**Odpovídající role:** Agent pro správu | Správce fakturace | Globální správce | Agent helpdesku | Sales agent | Správce správy uživatelů

Ceník nového komerčního prostředí Azure v CSP je zveřejněný v Partnerské centrum. Ceník se dynamicky doručuje v přesném souboru v reálném čase a ceny se zobrazují pouze v USD. Od 28. ledna 2021 se partnerům v oblasti EU/EFTA a Velké Británie, kteří mají nové zákazníky a stávající zákazníky CSP, kteří poprvé kupují nové obchodní nabídky, jejichž tenanti vytvořili před 11. květnem 2020, budou tyto nákupy účtovat v měně umístění partnera.  Partneři, kteří se nacházejí mimo oblast EU/EFTA a Spojené království, se budou dál účtovat v měně umístění partnera. Další informace najdete v článku [Plán Azure – fakturace.](azure-plan-billing.md)

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Informace o cenách předplatných najdete v tématu Ceny plánu Azure.

1. V nabídce Partnerské centrum na levé straně vyberte **Sell (Prodej)** a pak **vyberte Marketplace**.

2. V části Ceny plánu Azure vyberte zemi, pro kterou chcete cenu.

3. Vedle možnosti **Typ exportu** vyberte **Ceny spotřeby plánu Azure,** **Ceny rezervací** plánu Azure nebo **Kurzy FX.** 

>[!NOTE] 
>**Sazby FX** nejsou specifické pro jednotlivé země.

4. Vedle **položky Ceny pro datum** vyberte datum, které chcete, například **Aktuální**.

   :::image type="content" source="images/azure/pricingnew.png" alt-text="specifická pro zemi":::

>[!NOTE] 
>Můžete exportovat dva různé ceníky – ceny plánu Azure a ceny třetích stran na Marketplace.

## <a name="azure-price-list-specifics"></a>Specifika ceníku Azure

- Ceny plánu Azure budou k dispozici na stránce Marketplace v části Partnerské centrum v části **Prodej.**

- Exporty budou k dispozici pro služby využití plánu Azure, rezervace Azure a sazby FX.

- Mezi možnosti exportu patří:

  - **Today's pricing**: Zahrnuje všechny měřiče a ceny od 1. dne v měsíci až po aktuální datum aktuálního měsíce. To zahrnuje nové ceny, změněné ceny nebo odebrané ceny. Všechny ceny budou mít počáteční počáteční a koncové datum, které vysvětlí, jestli jsou nové nebo odebrané.

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
|Publisher|První stranou bude vždy Microsoft.|
|Popis Sku|Popis SKU|
|UnitOfMeasure|Jednotky, které se budou účtovat nebo fakturovat|
|TermDuration|U produktů založených na termínech se délka období vztahuje na rezervace.|
|Trhu|Trh cen|
|Měna|Měna cen|
|UnitPrice|Cena za jednotku|
|PricingTierRangeMin|Pro vrstvené ceny platí minimální cena.|
|PricingTierRangeMax|Pro vrstvené ceny platí maximální cena.|
|EffectiveStartDate|Počáteční datum cen|
|EffectiveEndDate|Koncové datum cen|
|ID měřiče|ID měřiče SKU produktu|
|MeterType (Typ měřiče)|Typ měřiče|
|Značky|Vlastnosti položky, u cen plánu Azure to budou Azure nebo Azure a rezervace (konkrétně rezervace).|

Ceníky pro plán Azure je možné exportovat na stránce [Ceny a nabídky v](https://partner.microsoft.com/dashboard/sell/pricingandoffers) Partnerské centrum.

## <a name="tiered-pricing"></a>Vrstvené ceny

Některé služby Využití plánu Azure podporují vrstvené ceny. Partneři najdou tyto produkty a SKU v ceníku plánu Azure. Položky, které mají hodnoty ve sloupcích s rozsahem cenových úrovní, umožňují partnerům pochopit cenu na základě využití. V následujícím příkladu s ukázkovými daty máme jednu SKU produktu se třemi cenovou úrovní.

|**Productid**   |**ID SKU**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
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
