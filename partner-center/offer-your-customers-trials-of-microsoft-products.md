---
title: Nabídnout zákazníkům zkušební verze produktů Microsoftu
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Umožněte zákazníkům vyzkoušení produktů předplatného Microsoft po dobu 30 dnů. Zaregistrujte si tyto bezplatné zkušební verze v katalogu stejně jako mnoho dalších online služby.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d6fda82464b9abc30714798a2ee3999d8f93db5
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151130"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Poskytněte zákazníkům 30denní bezplatné zkušební verze produktů Microsoftu

**Příslušné role**: globální správce | Správce správy uživatelů | Agent prodeje

Dobrým způsobem, jak zavést zákazníky do nových produktů Microsoftu, je nabízet bezplatné zkušební verze na 30 dní. Zkušební verze můžete zaregistrovat v katalogu stejně jako mnoho dalších online služby. Všichni partneři se můžou zúčastnit.

## <a name="available-trial-offers"></a>Dostupné zkušební nabídky

Všechny vaše bezplatné zkušební nabídky najdete na stránce **zákazníka** . Tato stránka obsahuje seznam všech předplatných včetně bezplatných zkušebních verzí a placených předplatných. (Tato funkce není aktuálně k dispozici v Číně.)

Každý zákazník má pro každou dostupnou nabídku nárok na jednu bezplatnou zkušební verzi. Můžou například získat jednu bezplatnou zkušební verzi pro Microsoft 365 Business Standard a jednu bezplatnou zkušební verzi pro Office 365 E3. Pokud však zákazník tuto nabídku již vlastní, nemůže použít bezplatnou zkušební verzi této nabídky.

### <a name="available-products"></a>Dostupné produkty

Bezplatné zkušební verze jsou k dispozici pro komplexnější a oblíbené nabídky založené na licesen. Nové zkušební nabídky mohou být zavedeny měsíčně.

Na stránce ceny **a nabídky** v partnerském centru můžou vyhledat zkušební verze v ceníku měsíčně. Nabídky zkušební verze budou obsahovat "zkušební verzi" uvedené ve sloupci **typ sekundární licence** na ceník.

V současné době nejsou **k dispozici žádné bezplatné zkušební** verze nabídek pro státní instituce, nabídek pro vzdělávání ani nabídek doplňků.

## <a name="licenses-for-free-trial-offers"></a>Licence na nabídky bezplatné zkušební verze

Všechny bezplatné zkušební verze poskytují 25 licencí. Toto číslo během zkušební verze nemůžete změnit. V bezplatné zkušební verzi nemůžete přidávat ani odebírat licence. Po převodu zkušební verze na placené předplatné můžete k předplatnému přidat další licence.

Zkušební licence by se měly uživatelům přiřažovat stejným způsobem, jakým se přiřazuje licence na placené služby.

## <a name="sign-customers-up-for-trials"></a>Registrace zákazníků ke zkušebním testům

Získejte zkušební verzi pro zákazníka v Partnerské centrum:

1. V **sell** on the Partnerské centrum (Prodej na Partnerské centrum) přejděte na **Catalog (Katalog).** 
2. V katalogu v části **Četnost fakturace** vyberte **Zkušební nabídka.** To umožňuje zobrazit a zakázat jenom bezplatné zkušební verze jiných nabídek, které nejsou bezplatné. Zkušební verze se zobrazí v **katalogu** na kartě Zkušební verze.
3. Vyberte bezplatnou zkušební verzi, kterou chcete nabídnout, a pak vyberte **odeslat**. Všechny zkušební verze jsou 30 dní, během kterých se vám neúčtuje. Můžete ho také kdykoli během zkušební verze převést na placené předplatné.

## <a name="converting-trials-to-paid-subscriptions"></a>Převod zkušebních období na placená předplatná

Bezplatná zkušební verze se automaticky převede na placené předplatné. Po 30 dnech je nutné bezplatnou zkušební verzi převést na placené předplatné, jinak [vyprší jeho platnost.](#expiring-offers) Bezplatné zkušební verze nelze prodloužit.

Tuto zkušební verzi budete muset převést na placené předplatné sami. Můžete to provést [pomocí partnerského centra](#convert-trials-using-partner-center) nebo [přes rozhraní API partnerského centra](#convert-trials-using-apis).

> [!NOTE]
> Bezplatné zkušební verze pro program poskytovatele Cloud Solution Provider (CSP) nelze převést na jiného tenanta programu (například EA, Open nebo MOSP).

### <a name="convert-trials-using-partner-center"></a>Převod zkušebních verzí pomocí partnerského centra

Zkušební verze můžete převést na placená předplatná pomocí partnerského centra:

1. Přejít na stránku předplatné zákazníka a vyberte bezplatnou zkušební verzi.
2. Vyberte **převést zkušební verzi na placené předplatné**.
3. Zadejte požadovaný počet licencí a četnost fakturace a pak vyberte **použít**.
4. Fakturace za placené předplatné začíná dnem převodu a předplatné automaticky obnoví 12 měsíců od data převodu. 

### <a name="convert-trials-using-apis"></a>Převod zkušebních verzí pomocí rozhraní API

Možná budete muset změnit rozhraní API tak, aby vyhovovala převodu bezplatné zkušební verze na placené předplatné. Další informace najdete v následující dokumentaci pro vývojáře:

- [Převod zkušební verze předplatného na placenou](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Získání seznamu nabídek převod zkušebních verzí](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Zkušební verze bez převodů

Ne všechny zkušební verze lze převést na placené odběry. Partneři můžou používat zkušební verzi, která nemá žádné převody do data vypršení platnosti. Partneři můžou zakoupit kompatibilní nabídky, které podporují stejné služby jako nabídka zkušební verze.  Tento postup by se měl provést před vypršením platnosti zkušební verze, aby se zajistilo, že nově zakoupené služby nabídek budou zarovnány se službami zkušební verze. 

|**Zkušební verze**   |**Kompatibilní nabídky malých firem**   |**Kompatibilní nabídky Enterprise**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Zkušební verze komerčního cloudu Microsoft Teams (zahájeného uživatelem)   |Microsoft 365 Business Basic, Microsoft 365 Business Standard, Microsoft 365 Business Premium   | F3 (dříve F1), Office 365 for Enterprise (E1, E3 a E5), Microsoft 365 F1/F3, Microsoft 365 Enterprise (E3)   |

>[!NOTE]
>Výše uvedené nabídky mají podobné plány služeb s podobnými funkcemi, ale mezi nabídkami mohou být některé rozdíly.

### <a name="expiring-offers"></a>Vypršení platnost nabídek

Na nabídky, které vyprší platnost, vám nebude oznámeno. Nadcházející data vypršení platnosti můžete sledovat pomocí zobrazení zákazníka na Partnerské centrum nebo dotazem rozhraní API. Je vhodné tato data často monitorovat, abyste při rozhodování mohli se zákazníky provést odpovídající následné akce.

Po vypršení platnosti zkušební verze se zákazníkovi, který se pokusí k této zkušební verzi přihlásit, zobrazí zpráva o vypršení platnosti. Data se ale ukládají v souladu se standardy uchovávání dat. Po zakoupení nového předplatného se stejnými plány služeb budou informace o zákazníkovi znovu dostupné z nově aktivovaného předplatného.

## <a name="billing"></a>Fakturace

Roční fakturace a bezplatné zkušební verze jsou stejné v suverénních cloudech i ve veřejném cloudu. Jediným rozdílem jsou skladové skladové verze zkušební verze, které jsou k dispozici v době uvedení na trh.

## <a name="billing-for-free-trials"></a>Fakturace bezplatných zkušebních období

Bezplatné zkušební verze je možné použít pro měsíční i roční fakturovaná předplatná. Frekvenci fakturace můžete vybrat při převodu zkušební verze na placené předplatné.

Počáteční datum předplatného je založené na datu převodu. Pokud se bezplatná zkušební verze převede na placenou nabídku s roční fakturací, datum prodloužení platnosti předplatného bude 12 měsíců od data převodu. Pokud se bezplatná zkušební verze převede na placenou nabídku s měsíční fakturací, datum prodloužení platnosti předplatného bude 12 měsíců od data fakturace následujícího po datu převodu.

### <a name="invoices"></a>Faktury

Na faktuře ani v souboru s vyrovnáním na základě licencí se nezískaly bezplatné zkušební verze. Bezplatné zkušební verze se zobrazí na faktuře a souboru s vyrovnáním na základě licencí až po převodu bezplatné zkušební verze na placené předplatné. Převedený odběr se zobrazí stejným způsobem jako jakékoli nové předplatné.

### <a name="incentives"></a>Pobídky

Bezplatné zkušební verze nemají dopad na pobídky.

## <a name="support"></a>Podpora

Pro podporu bezplatné zkušební verze odešlete žádost o služby prostřednictvím partnerského centra.