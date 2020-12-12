---
title: Běžné měsíční scénáře fakturace
ms.topic: article
ms.date: 05/13/2020
description: Obvyklé scénáře v partnerském centru při použití měsíční fakturace – zahrnuje přidání nových předplatných, změna počtu licencí a pozastavení předplatných.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 05c46faa3fd012677b615caa228cf4f7c6fe6c90
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354572"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Ukázky měsíčních scénářů fakturace pro nové předplatné, změna množství licencí nebo přerušení

**Příslušné role**

- Agent správce
- Správce fakturace
- Agent helpdesku
- Agent prodeje

Tyto příklady [běžných fakturačních scénářů](common-billing-scenarios.md) platí, pokud použijete měsíční fakturaci v partnerském centru.

## <a name="new-monthly-subscription"></a>Nové měsíční předplatné

Datum fakturace je 15. den v měsíci. 13. ledna zakoupíte nové předplatné s jednou licencí pro $4 měsíčně a vyberete možnost měsíční fakturace. 15. ledna se souborem odsouhlasení na základě licencí bude obsahovat následující fakturační řádky:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Poplatek za cyklus   |4,00       |1        |4,00 |

Soubor odsouhlasení založený na licencích z února v únoru bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Poplatek za cyklus   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Změnit množství licencí

Datum fakturace je 15. den v měsíci. 13. ledna zakoupíte nové předplatné s jednou licencí pro $4 měsíčně a vyberete možnost měsíční fakturace. 15. ledna se souborem odsouhlasení na základě licencí bude obsahovat následující fakturační řádky:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Poplatek za cyklus   |4,00       |1        |4,00    |

1. února zvýšíte počet licencí z jedné na dvě. Soubor odsouhlasení založený na licencích z února v únoru bude obsahovat následující fakturační řádky:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |Poměr instance cyklu   |-4,00       |1        |-4,00   |
|1/13/2018         |1/31/2018    | Poměr instance cyklu   |2.45       |1        |2.45    |
|2. 1. 2018         |2/12/2018    | Poměr instance cyklu   |1,55       |2        |3,10    |
|2/13/2018         |3/12/2018    | Poměr instance cyklu   |4,00       |2        |8,00    |

Měsíční cena je 4,00 a v období služby 1/13/2018 – 2/12/2018 je 31 dní. To je rovno denní ceně 0,129 (4/31).

V období probíhající 1/13/2018 – 1/31/2018 je 19 dnů.

Cena za jednotku pronákl = 2,451 = 19 × 0,129

V období probíhající 2/1/2018 – 2/12/2018 je 12 dnů.

Cena za jednotku mezidávkou = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Pozastavit před 30 dny

Datum fakturace je 15. den v měsíci. 13. ledna zakoupíte nové předplatné s jednou licencí pro $4 měsíčně a vyberete možnost měsíční fakturace. 15. ledna se souborem odsouhlasení na základě licencí bude obsahovat následující fakturační řádky:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Poplatek za cyklus   |4,00       |1        |4,00    |

1. února jste odzastavili předplatné. Soubor odsouhlasení založený na licencích z února v únoru bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Zrušit poplatek|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Pozastavit po 30 dnech

Datum fakturace je 15. den v měsíci. 13. ledna zakoupíte nové předplatné s jednou licencí pro $4 měsíčně a vyberete možnost měsíční fakturace. 15. ledna se souborem odsouhlasení na základě licencí bude obsahovat následující fakturační řádky:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Poplatek za cyklus|4,00|1|4,00

Soubor odsouhlasení založený na licencích z února v únoru bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Poplatek za cyklus|4,00|1|4,00

1. března přerušíte předplatné. Ne15. března soubor odsouhlasení s licencí bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Zrušit poplatek|-1,72|1|-1,72

Měsíční cena je 4,00 a v období služby 2/13/2018 – 3/12/2018 je 28 dnů. To je rovno denní ceně 0,143 (4/28).

Cena za jednotku = dny v období služby × denní cena × počet licencí.

V období zrušení 3/1/2018 – 3/12/2018 je k dispozici 12 dní.

Proto Jednotková cena =-1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Další kroky

- [Scénáře fakturace v jednom čase a výběr opakujících se nákupu](common-billing-scenarios-onetime-recurring.md)