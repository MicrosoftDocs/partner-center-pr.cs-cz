---
title: Roční fakturace – běžné scénáře
ms.topic: article
ms.date: 05/05/2020
description: Roční fakturace z partnerského centra – když přidáváte nové odběry, přidáte licence před datum fakturace, změníte množství licencí nebo pozastavit/znovu aktivujete odběry.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 086a7d359e1b903684af4ecddac37eda584e55f8
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/17/2020
ms.locfileid: "92527022"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Běžné roční fakturační scénáře v partnerském centru

**Příslušné role**

- Agent správce
- Správce fakturace
- Agent helpdesku
- Agent prodeje

Tyto příklady [běžných fakturačních scénářů](common-billing-scenarios.md) platí, pokud použijete roční fakturaci v partnerském centru.

## <a name="new-annual-subscription"></a>Nové roční předplatné

Datum fakturace je 15. den v měsíci. 13. ledna zakoupíte nové předplatné s jednou licencí pro $4 měsíčně a vyberete roční fakturaci. 15. ledna se souborem odsouhlasení na základě licencí bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Poměrné poplatky při nákupu|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Přidat licenci po datu výročí předplatného, ale před datem fakturace

Koupíte nové předplatné na 2/11/17 s jednou licencí pro $211.20/year. Předplatné vašeho předplatného je nastavené na 11. den v měsíci. Fakturační systém Microsoftu vytvoří následující fakturační řádky:

- $211,20 poplatek za období 2/11/17 – 2/10/18.

2/12/17 si koupíte druhou licenci. Datum fakturace je 2/14/17. Vygeneruje se soubor faktury a odsouhlasení. Soubor pro odsouhlasení bude obsahovat následující fakturační řádky:

|Počáteční datum platby  |Koncové datum zpoplatnění  |Typ poplatků  |Cena za jednotku |Množství | Částka |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Poměrné poplatky při nákupu |211,20 |1 | 211,20 |

V rámci vašeho předplatného, 3/11/17, fakturační systém Microsoftu vytvoří následující fakturační řádky pro zvýšení licence na 2/12/17:

- $211,20 kredit za období 2/11/17 – 2/10/18.
- $0,58 sazba za licenci na 1 licenci za období 2/11/17 – 2/11/17.
- $15,62 sazba za licenci na 2 licence za období 2/12/17 – 3/10/2017.
- $195,00 sazba za licenci na 2 licence za období 3/11/2017 – 2/10/2018.

2/11/17 zakoupíte předplatné. 2/12/17 můžete přidat licenci. Datum fakturace je 2/14/17. V 2/11/18 se vaše předplatné obnovuje.

Vaše další datum fakturace je 3/14/17 a vygeneruje se soubor pro odsouhlasení & faktury. Soubor pro odsouhlasení bude obsahovat následující fakturační řádky:

|Počáteční datum platby  |Koncové datum zpoplatnění  |Typ poplatků  |Cena za jednotku |Množství | Částka |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Poměr instance cyklu |-211,20 |1 |-211,20 |
|2/11/2017 |2/11/2017 |Poměr instance cyklu |0,58 |1 |0,58 |
|2/12/2017 |3/10/2017 |Poměr instance cyklu |15,62 |2 |31,25 |
|3/11/2017 |2/10/2018 |Poměr instance cyklu |195,00 |2 |390,00 |

V 2/11/18 se předplatné obnovuje na další 12 měsíců.

## <a name="change-license-quantity"></a>Změnit počet licencí

Datum fakturace je 15. den v měsíci. 13. ledna zakoupíte nové předplatné s jednou licencí pro $4 měsíčně a vyberete roční fakturaci. 15. ledna se souborem odsouhlasení na základě licencí bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Poměrné poplatky při nákupu|48,00|1|48,00

1. února zvýšíte počet licencí z jedné na dvě. Soubor odsouhlasení založený na licencích z února v únoru bude obsahovat následující fakturační řádky:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Poměr instance cyklu|-48,00|1|-48,00
1/13/2018|1/31/2018|Poměr instance cyklu|2,47|1|2,47
2. 1. 2018|1/12/2019|Poměr instance cyklu|44,98|2|89,96

Roční cena je 48,00, což odpovídá denní ceně 0,13 (48.00/365).

Cena za jednotku = dny v období služby × denní cena × počet licencí.

Období služby 1/13/2018 – 1/31/2018 obsahuje 19 dnů.

Proto Jednotková cena = 2,47 (19x 0.13 x1)

V období služby 2/1/2018 – 1/12/2019 je 346 dní.

Proto Jednotková cena = 44,98 (346x 0.13 X2)

## <a name="suspend-before-30-days"></a>Pozastavit před 30 dny

Datum fakturace je 15. den v měsíci. 13. ledna zakoupíte nové předplatné s jednou licencí pro $4 měsíčně a vyberete roční fakturaci. 15. ledna se souborem odsouhlasení na základě licencí bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Poměrné poplatky při nákupu|48,00|1|48,00

1. února vaše předplatné zastavíte. Soubor odsouhlasení založený na licencích z února v únoru bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Zrušit poplatek|-48,00|1|-48,00

## <a name="suspend-after-30-days"></a>Pozastavit po 30 dnech

Datum fakturace je 15. den v měsíci. 13. ledna zakoupíte nové předplatné s jednou licencí pro $4 měsíčně a vyberete roční fakturaci. 15. ledna se souborem odsouhlasení na základě licencí bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Poměrné poplatky při nákupu|48,00|1|48,00

Soubor odsouhlasení založený na licencích s únorem v únoru nebude obsahovat žádné fakturační řádky pro toto předplatné.
1. března vaše předplatné zastavíte. Ne15. března soubor odsouhlasení s licencí bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Zrušit poplatek|-41,34|1|-41,34

Roční cena je 48,00, což odpovídá denní ceně 0,13 (48.00/365).

Cena za jednotku = dny v období služby × denní cena × počet licencí.

V období služby 3/1/2018 – 1/12/2019 je 318 dní.

Proto Jednotková cena = 41,34 (318x 0.13 x1). Vzhledem k tomu, že se jedná o kredit, je jednotková cena-41,34.

## <a name="suspend-and-reactivate"></a>Pozastavit a znovu aktivovat

Datum fakturace je 15. den v měsíci. 13. ledna zakoupíte nové předplatné s jednou licencí pro $4 měsíčně a vyberete roční fakturaci. 15. ledna se souborem odsouhlasení na základě licencí bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Poměrné poplatky při nákupu|48,00|1|48,00

1. února vaše předplatné zastavíte. Soubor odsouhlasení založený na licencích z února v únoru bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Zrušit poplatek|-48,00|1|-48,00

1. března znovu aktivujete své předplatné. Ne15. března soubor odsouhlasení s licencí bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Poměrné poplatky při nákupu|41,34|1|41,34

Roční cena je 48,00, což odpovídá denní ceně 0,13 (48.00/365).

Cena za jednotku = dny v období služby × denní cena × počet licencí.

V období služby 3/1/2018 – 1/12/2019 je 318 dní.

Proto Jednotková cena = 41,34 (318x 0.13 x1).
