---
title: Běžné měsíční scénáře fakturace
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obvyklé scénáře v partnerském centru při použití měsíční fakturace – zahrnuje přidání nových předplatných, změna počtu licencí a pozastavení předplatných.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 66c9ec09f707d87248fdef31e4cf66f4ca927ce1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148648"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Ukázky měsíčních scénářů fakturace pro nové předplatné, změna množství licencí nebo přerušení

**Příslušné role**: Agent správce | Správce fakturace | Agent helpdesku | Agent prodeje

Tyto příklady [běžných fakturačních scénářů](common-billing-scenarios.md) platí, pokud použijete měsíční fakturaci v partnerském centru.

## <a name="new-monthly-subscription"></a>Nové měsíční předplatné

Datum fakturace je 15. den v měsíci. 13. ledna jste si koupili nové předplatné s jednou licencí pro $4 měsíčně a vybrali možnost měsíční fakturace. 15. ledna – soubor odsouhlasení na základě licence bude obsahovat následující fakturační řádky:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Poplatek za cyklus   |4,00       |1        |4,00 |

Soubor odsouhlasení založený na licencích bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Poplatek za cyklus   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Změnit množství licencí

Vaše fakturační datum je 15. dne každého měsíce. 13. ledna si zakoupíte nové předplatné s jednou licencí za 4 USD za měsíc a vyberete měsíční fakturaci. Soubor s vyrovnáním založeným na licencích k 15. lednu bude obsahovat následující fakturační řádky:

|Počáteční datum poplatku |Charge End Date |Typ poplatku |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Poplatek za cyklus   |4,00       |1        |4,00    |

1. února zvýšíte počet licencí z jednoho na dva. Soubor s vyrovnáním na základě licencí od 15. února bude obsahovat následující fakturační řádky:

|Počáteční datum poplatku |Charge End Date |Typ poplatku |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |Cycle Instance Prorate   |-4.00       |1        |-4,00   |
|1/13/2018         |1/31/2018    | Poměr instance cyklu   |2.45       |1        |2.45    |
|2. 1. 2018         |2/12/2018    | Poměr instance cyklu   |1,55       |2        |3,10    |
|2/13/2018         |3/12/2018    | Poměr instance cyklu   |4,00       |2        |8,00    |

Měsíční cena je 4,00 a v období služby 1/13/2018 – 2/12/2018 je 31 dní. To je rovno denní ceně 0,129 (4/31).

V období probíhající 1/13/2018 – 1/31/2018 je 19 dnů.

Cena za jednotku pronákl = 2,451 = 19 × 0,129

V období probíhající 2/1/2018 – 2/12/2018 je 12 dnů.

Cena za jednotku mezidávkou = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Pozastavit před 30 dny

Datum fakturace je 15. den v měsíci. 13. ledna jste si koupili nové předplatné s jednou licencí pro $4 měsíčně a vybrali možnost měsíční fakturace. Soubor s vyrovnáním založeným na licencích k 15. lednu bude obsahovat následující fakturační řádky:

|Počáteční datum poplatku |Charge End Date |Typ poplatku |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Poplatek za cyklus   |4,00       |1        |4,00    |

1. února pozastavíte předplatné. Soubor s vyrovnáním na základě licencí za 15. února bude obsahovat následující fakturační řádek:

|Počáteční datum poplatku |Charge End Date |Typ poplatku |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Poplatek za zrušení|-4.00|1|-4.00

## <a name="suspend-after-30-days"></a>Pozastavení po 30 dnech

Vaše fakturační datum je 15. dne každého měsíce. 13. ledna si zakoupíte nové předplatné s jednou licencí za 4 USD za měsíc a vyberete měsíční fakturaci. 15. ledna – soubor odsouhlasení na základě licence bude obsahovat následující fakturační řádky:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Poplatek za cyklus|4,00|1|4,00

Soubor odsouhlasení založený na licencích bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Poplatek za cyklus|4,00|1|4,00

Od 1. března můžete pozastavit odběr. 15. března soubor odsouhlasení na základě licence bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Poplatek za zrušení|-1.72|1|-1.72

Měsíční cena je 4,00 a v období služby je 13. 2. 2018 – 12. 3. 2018. To se rovná denní ceně 0,143 (4/28).

Jednotková cena = dny v období služby × denní cena × počet licencí.

V období zrušení je 1. 3. 2018– 12. 3. 2018 12. 2018.

Proto jednotková cena = -1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Další kroky

- [Scénáře fakturace pro jednou a výběr opakovaných nákupů](common-billing-scenarios-onetime-recurring.md)