---
title: Roční fakturace – běžné scénáře
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Partnerské centrum roční fakturace – když přidáte nová předplatná, přidejte licence před datem fakturace, změňte množství licencí nebo pozastavíte/znovu aktivujte předplatná.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a6392094e000b899e0545655ecf9ed6117535f7f
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148699"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Běžné scénáře roční fakturace v Partnerské centrum

**Odpovídající role:** Agent pro správu | Správce fakturace | Agent helpdesku | Agent prodeje

Tyto příklady [běžných fakturačních](common-billing-scenarios.md) scénářů platí, pokud používáte roční fakturaci v Partnerské centrum.

## <a name="new-annual-subscription"></a>Nové roční předplatné

Vaše fakturační datum je 15. dne každého měsíce. 13. ledna si zakoupíte nové předplatné s jednou licencí za 4 USD měsíčně a vyberete roční fakturaci. Soubor s vyrovnáním založeným na licencích k 15. lednu bude obsahovat následující fakturační řádek:

|Počáteční datum poplatku |Charge End Date |Typ poplatku |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Poplatky za přenos při nákupu|48.00|1|48.00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Přidání licence po datu výročí předplatného, ale před datem fakturace

Nové předplatné zakoupíte 11. 2. 2019 s jednou licencí na 211,20 USD za rok. Vaše výročí předplatného je nastavené na 11. den každého měsíce. Fakturační systém Microsoftu vytvoří následující fakturační řádky:

- $211,20 poplatek za období 2/11/17 – 2/10/18.

Na 2/12/17 si koupíte druhou licenci. Datum fakturace je 2/14/17. Vygeneruje se soubor faktury a odsouhlasení. Soubor pro odsouhlasení bude obsahovat následující fakturační řádky:

|Počáteční datum platby  |Koncové datum zpoplatnění  |Typ poplatků  |Cena za jednotku |Množství | Částka |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Poměrné poplatky při nákupu |211,20 |1 | 211,20 |

V rámci vašeho předplatného, 3/11/17, fakturační systém Microsoftu vytvoří následující fakturační řádky pro zvýšení licence na 2/12/17:

- $211,20 kredit za období 2/11/17 – 2/10/18.
- $0,58 sazba za licenci na jednu licenci pro období 2/11/17 – 2/11/17.
- $15,62 sazba za licenci na dvě licence za období 2/12/17 – 3/10/2017.
- $195,00 sazba za licenci na dvě licence za období 3/11/2017 – 2/10/2018.

Na 2/11/17 si koupíte předplatné. 12. 2. 2017 přidáte licenci. Vaše fakturační datum je 14. 2. 2017. 11. 2. 2018 se vaše předplatné prodlužuje.

Další fakturační datum je 14. 3. 2017 a vygeneruje se soubor faktury a odsouhlasení. Soubor s vyrovnáním bude obsahovat následující fakturační řádky:

|Počáteční datum poplatku  |Charge End Date  |Typ poplatku  |Cena za jednotku |Množství | Částka |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Cycle Instance Prorate |-211.20 |1 |-211.20 |
|2/11/2017 |2/11/2017 |Cycle Instance Prorate |0.58 |1 |0.58 |
|2/12/2017 |3/10/2017 |Poměr instance cyklu |15,62 |2 |31,25 |
|3/11/2017 |2/10/2018 |Poměr instance cyklu |195,00 |2 |390,00 |

V 2/11/18 se předplatné obnovuje na další 12 měsíců.

## <a name="change-license-quantity"></a>Změnit množství licencí

Datum fakturace je 15. den v měsíci. 13. ledna jste si koupili nové předplatné s jednou licencí pro $4 měsíčně a vybrali roční fakturaci. 15. ledna se souborem odsouhlasení na základě licencí bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Poměrné poplatky při nákupu|48,00|1|48,00

1. února zvýšíte počet licencí z jednoho na dva. Soubor s vyrovnáním na základě licencí od 15. února bude obsahovat následující fakturační řádky:

|Počáteční datum poplatku |Charge End Date |Typ poplatku |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Cycle Instance Prorate|-48.00|1|-48.00
1/13/2018|1/31/2018|Cycle Instance Prorate|2.47|1|2.47
2. 1. 2018|1/12/2019|Cycle Instance Prorate|44.98|2|89.96

Roční cena je 48,00, což se rovná denní ceně 0,13 (48,00/365).

Cena za jednotku = dny v období služby × denní cena × počet licencí.

Období služby 1/13/2018 – 1/31/2018 obsahuje 19 dnů.

Proto Jednotková cena = 2,47 (19x 0.13 x1)

V období služby 2/1/2018 – 1/12/2019 je 346 dní.

Proto Jednotková cena = 44,98 (346x 0.13 X2)

## <a name="suspend-before-30-days"></a>Pozastavit před 30 dny

Datum fakturace je 15. den v měsíci. 13. ledna jste si koupili nové předplatné s jednou licencí pro $4 měsíčně a vybrali roční fakturaci. 15. ledna se souborem odsouhlasení na základě licencí bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Poměrné poplatky při nákupu|48,00|1|48,00

1. února vaše předplatné zastavíte. Soubor odsouhlasení založený na licencích bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Charge End Date |Typ poplatku |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Poplatek za zrušení|-48.00|1|-48.00

## <a name="suspend-after-30-days"></a>Pozastavení po 30 dnech

Vaše fakturační datum je 15. dne každého měsíce. 13. ledna si zakoupíte nové předplatné s jednou licencí za 4 USD za měsíc a vyberete roční fakturaci. Soubor s vyrovnáním založeným na licencích k 15. lednu bude obsahovat následující fakturační řádek:

|Počáteční datum poplatku |Charge End Date |Typ poplatku |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Poplatky za přenos při nákupu|48.00|1|48.00

Soubor s vyrovnáním na základě licencí z 15. února nebude obsahovat žádné fakturační řádky pro toto předplatné.
1. března vaše předplatné zastavíte. 15. března soubor odsouhlasení na základě licence bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Zrušit poplatek|-41,34|1|-41,34

Roční cena je 48,00, což odpovídá denní ceně 0,13 (48.00/365).

Cena za jednotku = dny v období služby × denní cena × počet licencí.

V období služby 3/1/2018 – 1/12/2019 je 318 dní.

Proto Jednotková cena = 41,34 (318x 0.13 x1). Vzhledem k tomu, že se jedná o kredit, je jednotková cena-41,34.

## <a name="suspend-and-reactivate"></a>Pozastavit a znovu aktivovat

Datum fakturace je 15. den v měsíci. 13. ledna jste si koupili nové předplatné s jednou licencí pro $4 měsíčně a vybrali roční fakturaci. 15. ledna se souborem odsouhlasení na základě licencí bude obsahovat následující fakturační řádek:

|Počáteční datum platby |Charge End Date |Typ poplatku |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Poplatky za přenos při nákupu|48.00|1|48.00

1. února pozastavíte předplatné. Soubor s vyrovnáním na základě licencí za 15. února bude obsahovat následující fakturační řádek:

|Počáteční datum poplatku |Charge End Date |Typ poplatku |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Poplatek za zrušení|-48.00|1|-48.00

1. března znovu aktivujte své předplatné. Soubor s vyrovnáním na základě licencí k 15. březnu bude obsahovat následující fakturační řádek:

|Počáteční datum poplatku |Koncové datum zpoplatnění |Typ poplatků |Cena za jednotku |Množství |Částka |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Poměrné poplatky při nákupu|41,34|1|41,34

Roční cena je 48,00, což odpovídá denní ceně 0,13 (48.00/365).

Cena za jednotku = dny v období služby × denní cena × počet licencí.

V období služby 3/1/2018 – 1/12/2019 je 318 dní.

Proto Jednotková cena = 41,34 (318x 0.13 x1).
