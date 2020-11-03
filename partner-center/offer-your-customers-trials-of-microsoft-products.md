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
ms.openlocfilehash: a51504a5e560f8a8041c448c3e5d9e7f0cfdae07
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527295"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Poskytněte zákazníkům 30denní bezplatné zkušební verze produktů Microsoftu

**Platí pro**

- Partnerské centrum

**Příslušné role**
-   Globální správce 
-   Správce uživatelů
-   Agent prodeje

Dobrým způsobem, jak zavést zákazníky do nových produktů Microsoftu, je nabízet bezplatné zkušební verze na 30 dní. Zkušební verze můžete zaregistrovat v katalogu stejně jako mnoho dalších online služby. Všichni partneři se můžou zúčastnit.

## <a name="available-trial-offers"></a>Dostupné zkušební nabídky

Všechny vaše bezplatné zkušební nabídky najdete na stránce **zákazníka** . Tato stránka obsahuje seznam všech předplatných včetně bezplatných zkušebních verzí a placených předplatných. (Tato funkce není aktuálně k dispozici v Číně.)

Každý zákazník má pro každou dostupnou nabídku nárok na jednu bezplatnou zkušební verzi. Můžou například získat jednu bezplatnou zkušební verzi pro Microsoft 365 Business Standard a jednu bezplatnou zkušební verzi pro Office 365 E3. Pokud však zákazník tuto nabídku již vlastní, nemůže použít bezplatnou zkušební verzi této nabídky.

### <a name="available-products"></a>Dostupné produkty

Bezplatné zkušební verze jsou k dispozici pro komplexnější a oblíbené nabídky založené na licesen. Nové zkušební nabídky mohou být zavedeny měsíčně.

Na stránce ceny **a nabídky** v partnerském centru můžou vyhledat zkušební verze v ceníku měsíčně. Nabídky zkušební verze budou obsahovat "zkušební verzi" uvedené ve sloupci **typ sekundární licence** na ceník.

V současné době nejsou k dispozici **žádné bezplatné zkušební** verze pro nabídky státní správy, nabídky vzdělávání nebo nabídky doplňků.

## <a name="licenses-for-free-trial-offers"></a>Licence pro nabídky bezplatné zkušební verze

Všechny bezplatné zkušební verze poskytují 25 licencí. Během zkušebního období nemůžete toto číslo změnit. V bezplatné zkušební verzi nemůžete přidávat ani odebírat licence. Po převedení zkušební verze na placené předplatné můžete do předplatného přidat další licence.

Zkušební licence by se měly přiřazovat uživatelům stejným způsobem, jakým se přiřadí licence k placeným službám.

## <a name="sign-customers-up-for-trials"></a>Podepsat zákazníky do zkušební verze

Získejte zkušební verzi pro zákazníka v partnerském centru:

1. V části **prodej** v partnerském centru můžete přejít na **katalog** . 
2. V katalogu, z **četnosti fakturace** , klikněte na **nabídku zkušební verze** . Tato možnost umožňuje zobrazit pouze bezplatné zkušební verze a zakáže jiné nabídky, které nejsou bezplatné. Zkušební verze se zobrazí na kartě **zkušební** verze v katalogu.
3. Vyberte bezplatnou zkušební verzi, kterou chcete nabídnout, a pak vyberte **Odeslat** . Všechny zkušební verze jsou po dobu třiceti dnů, během kterých se vám neúčtují poplatky. Můžete ho také převést na placené předplatné kdykoli během zkušebního období.

## <a name="converting-trials-to-paid-subscriptions"></a>Převádění zkušebních verzí na placené odběry

Bezplatná zkušební verze se automaticky nepřevede na placené předplatné. Po 30 dnech se bezplatná zkušební verze musí převést na placené předplatné nebo [vyprší platnost](#expiring-offers). Bezplatné zkušební verze nelze rozšířit.

Tuto zkušební verzi budete muset převést na placené předplatné sami. Můžete to provést [pomocí partnerského centra](#convert-trials-using-partner-center) nebo [přes rozhraní API partnerského centra](#convert-trials-using-apis).

> [!NOTE]
> Bezplatné zkušební verze pro program poskytovatele Cloud Solution Provider (CSP) nelze převést na jiného tenanta programu (například EA, Open nebo MOSP).

### <a name="convert-trials-using-partner-center"></a>Převod zkušebních verzí pomocí partnerského centra

Zkušební verze můžete převést na placená předplatná pomocí partnerského centra:

1. Přejít na stránku předplatné zákazníka a vyberte bezplatnou zkušební verzi.
2. Vyberte **převést zkušební verzi na placené předplatné** .
3. Zadejte požadovaný počet licencí a četnost fakturace a pak vyberte **použít** .
4. Vyúčtování placeného předplatného začíná na datu převodu a předplatné se na základě data konverze obnoví dvanáct měsíců. 

### <a name="convert-trials-using-apis"></a>Převod zkušebních verzí pomocí rozhraní API

Možná budete muset změnit rozhraní API tak, aby vyhovovala převodu bezplatné zkušební verze na placené předplatné. Další informace najdete v následující dokumentaci pro vývojáře:

- [Převod zkušebního předplatného na placené](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Získat seznam nabídek zkušebního převodu](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Zkušební verze bez převodů

Ne všechny zkušební verze lze převést na placené odběry. Partneři můžou používat zkušební verzi, která nemá žádné převody do data vypršení platnosti. Partneři můžou zakoupit kompatibilní nabídky, které podporují stejné služby jako nabídka zkušební verze.  Tento postup by se měl provést před vypršením platnosti zkušební verze, aby se zajistilo, že nově zakoupené služby nabídek budou zarovnány se službami zkušební verze. 

|**Zkušební verze**   |**Kompatibilní nabídky malých firem**   |**Kompatibilní nabídky Enterprise**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Zkušební verze komerčního cloudu Microsoft Teams (zahájeného uživatelem)   |Microsoft 365 Business Basic, Microsoft 365 Business Standard, Microsoft 365 Business Premium   | F3 (dříve F1), Office 365 for Enterprise (E1, E3 a E5), M365 F1/F3, M365 Enterprise (E3)   |

>[!NOTE]
>Výše uvedené nabídky mají podobné plány služeb s podobnými funkcemi, ale může to být několik rozdílů mezi nabídkami.

### <a name="expiring-offers"></a>Nabídky s vypršenou platností

Nebudete dostávat oznámení o nabídkách vypršení platnosti. Nadcházející data vypršení platnosti můžete sledovat pomocí zobrazení zákazníka v partnerském centru nebo dotazování rozhraní API. Je vhodné pravidelně monitorovat tato data, abyste mohli při přístupu k určitému bodu přijmout příslušné následné akce se zákazníky.

Po vypršení platnosti zkušební verze se zákazníkovi, který se pokusí přihlásit k této zkušební verzi, zobrazí zpráva o vypršení platnosti. Data se ale ukládají v souladu s standardy uchovávání dat. Po zakoupení nového předplatného se stejnými plány služeb můžete získat z nově aktivovaného předplatného i informace o zákazníkovi.

## <a name="billing"></a>Fakturace

Roční fakturace a bezplatné zkušební verze jsou pro cloudy v svrchovaném a veřejném cloudu stejné. Jediným rozdílem je počet SKU zkušební verze, které jsou k dispozici v době spuštění.

## <a name="billing-for-free-trials"></a>Fakturace za bezplatné zkušební verze

Bezplatné zkušební verze se dají použít pro měsíční i roční předplatné. Četnost fakturace můžete vybrat, když převedete zkušební verzi na placené předplatné.

Počáteční datum odběru vychází z data převodu. Pokud je bezplatná zkušební verze převedená na placenou nabídku s ročním vyúčtováním, bude datum obnovení předplatného 12 měsíců od data převodu. Pokud je bezplatná zkušební verze převedená na placenou nabídku s měsíčním účtováním, bude datum obnovení předplatného 12 měsíců od data fakturace po datu převodu.

### <a name="invoices"></a>Faktury

Neuvidíte bezplatné zkušební verze uvedené ve vaší faktuře nebo souboru pro odsouhlasení na základě licence. Bezplatné zkušební verze se zobrazí jenom v souboru odsouhlasení na faktuře a na základě licencí po převedení bezplatné zkušební verze na placené předplatné. Převedený odběr se zobrazí stejným způsobem jako jakékoli nové předplatné.

### <a name="incentives"></a>Uživatelům

Bezplatné zkušební verze nemají dopad na pobídky.

## <a name="support"></a>Podpora

Pro podporu bezplatné zkušební verze odešlete žádost o služby prostřednictvím partnerského centra.