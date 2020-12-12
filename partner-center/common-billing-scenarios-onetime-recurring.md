---
title: Fakturace jednorázovým &m periodickým nákupem
ms.topic: article
ms.date: 05/05/2020
description: Ukázky fakturace z partnerského centra pro jednorázové a výběr opakujících se nákupu – při nákupu předplatných můžete přidat další předplatná, přidat nebo odebrat licence.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a301aa85310142b3327baabbf3c8545b31f489bd
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354385"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Scénáře fakturace partnerského centra pro jednorázové a výběr opakujících se nákupu

**Příslušné role**

- Agent správce
- Správce fakturace
- Agent helpdesku
- Agent prodeje

Jedná se o [běžné scénáře fakturace](common-billing-scenarios.md). 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Zakupte si předplatné a přidejte licenci za stejný den.

Ve scénáři 1 si koupíte předplatné v 11. června za jednotkovou cenu $4. Později stejný den si koupíte jiné předplatné stejného předplatného, za stejnou cenu.

Soubor rekognoskaci bude obsahovat následující:

- $4 fakturace za službu v období od 10. července 9.
- %-4,00 poměrné refakturaci za službu období 11. června 11. Toto je období, kdy jste měli licenci 1. Výpočet = (měsíční cena/celkové dny v období služby) × dny v poměru periody služby x počet licencí = (4/30) × 30 × 1 = 4,00.
- $8,00 poměrné přeúčtování za období služby od 10. července 9. Toto je období, kdy máte 2 licence. Calculation = (4/30) × 30 × 2 = 8,00.

|**Datum nákupu**   |**Začátek platby** |**Konec zpoplatnění**  |**Cena za jednotku**  |**Množství**  |**Částka** |**Typ poplatku** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |1                 |$4            |Nová         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$4       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$8         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Koupit předplatné a později přidat další odběry

Ve scénáři 2 si koupíte předplatné v 11. června za jednotkovou cenu $4 a 12. června si koupíte pro stejný produkt za stejnou cenu jiné předplatné.

Soubor rekognoskaci bude obsahovat následující:

- $4 fakturace za službu v období od 10. července 9.
- %-3,87 poměrné přeúčtování za službu pro období služby 11. června – 12. června. Toto je období, kdy jste měli licenci 1. Výpočet = (měsíční cena/celkový počet dnů v období služby) × dní v poměru periody služby x počet licencí = (4/30) × 29 × 1 = 3,87.
- $7,74 poměrná částka za službu po dobu 12. července 9. Toto je období, kdy máte 2 licence. Calculation = (4/30) × 29 × 2 = 7,74.

|**Datum nákupu**   |**Začátek platby** |**Konec zpoplatnění**  |**Cena za jednotku**  |**Množství**  |**Částka** |**Typ poplatku** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (máte jednu licenci)     |6/10/2019   |7/09/2019         |$4         |1        |$4            |Nová         |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$3,87       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$7,74       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Koupit předplatné a odebrat licenci ke stejnému dni

Ve scénáři 3 si do 11. června zakoupíte pro stejný produkt dvě předplatná za jednotkovou cenu $4. Později stejný den odebíráte jednu z licencí.  

Soubor rekognoskaci bude obsahovat následující:

- $8 fakturace za dvě licence pro období služby od 10. července 9.
- %-8,00 poměrné refakturaci za službu období 11. června 11. Toto je období, kdy máte 2 licence. Výpočet = (měsíční cena/celkové dny v období služby) × dny v poměru periody služby x počet licencí = (4/30) × 30 × 2 = 8,00.
- $4,00 poměrná částka za službu v období od 11. června 9. Toto je období, kdy jste měli licenci 1. Calculation = (4/30) × 30 × 1 = 4,00.

|**Datum nákupu**   |**Začátek platby** |**Konec zpoplatnění**  |**Cena za jednotku**  |**Množství**  |**Částka** |**Typ poplatku** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |2                 |$8            |Nová         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$8       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 1      |$4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Zakoupení předplatného a pozdější odebrání licencí

Ve scénáři 4 si koupíte 2 odběry od 11. června za jednotkovou cenu $4 a 12. června odeberu jednu z licencí.

Soubor rekognoskaci bude obsahovat následující:

- $8 fakturace za službu v období od 10. července 9.
- %-7,74 poměrné přeúčtování za službu pro období služby 11. června – 12. června. Toto je období, kdy máte 2 licence. Výpočet = (měsíční cena/celkový počet dnů v období služby) × dní v poměru periody služby x počet licencí = (4/30) × 29 × 2 = 7,74.
- $3,87 poměrná částka za službu po dobu 12. července 9. Toto je období, kdy jste měli licenci 1. Calculation = (4/30) × 29 × 1 = 3,87.

|**Datum nákupu**   |**Začátek platby** |**Konec zpoplatnění**  |**Cena za jednotku**  |**Množství**  |**Částka** |**Typ poplatku** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (máte 2 licence)     |6/10/2019   |7/09/2019         |$4         |2        |$8       |Nová       |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$7,74       |removeQuantity           |
|6/12/2019 (máte licenci 1)    | 6/10/2019    |7/09/2019   |$4    |1      |$3,87    |removeQuantity |

## <a name="next-steps"></a>Další kroky

- [Ukázky měsíčních scénářů fakturace pro nové předplatné, změna množství licencí nebo přerušení](common-billing-scenarios-monthly.md)