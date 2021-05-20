---
title: Fakturace jednorázovým &m periodickým nákupem
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ukázky fakturace z partnerského centra pro jednorázové a výběr opakujících se nákupu – při nákupu předplatných můžete přidat další předplatná, přidat nebo odebrat licence.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a26b6e5299c5186959612e622808161ca0f7f7c2
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148614"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Scénáře fakturace partnerského centra pro jednorázové a výběr opakujících se nákupu

**Příslušné role**: Agent správce | Správce fakturace | Agent helpdesku | Agent prodeje

Jedná se o [běžné scénáře fakturace](common-billing-scenarios.md). 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Zakupte si předplatné a přidejte licenci za stejný den.

Ve scénáři 1 si koupíte předplatné v 11. června za jednotkovou cenu $4. Později stejný den si koupíte jiné předplatné stejného předplatného, za stejnou cenu.

Soubor rekognoskaci bude obsahovat následující:

- $4 fakturace za službu v období od 10. července 9.
- %-4,00 poměrné refakturaci za službu období 11. června 11. Toto je období, kdy jste měli licenci. Výpočet = (měsíční cena/celkové dny v období služby) × dny v poměru periody služby x počet licencí = (4/30) × 30 × 1 = 4,00.
- $8,00 poměrné přeúčtování za období služby od 10. července 9. Toto je období, kdy byste měli mít dvě licence. Calculation = (4/30) × 30 × 2 = 8,00.

|**Datum nákupu**   |**Začátek platby** |**Konec zpoplatnění**  |**Cena za jednotku**  |**Množství**  |**Částka** |**Typ poplatku** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |4 USD                |1                 |4 USD            |Nová         |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 USD        |1        | -$4       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 USD        | 2      |8 USD         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Nákup předplatného a přidání dalších předplatných později

Ve scénáři 2 zakoupíte předplatné 11. června za jednotkovou cenu 4 USD a 12. června zakoupíte další předplatné pro stejný produkt za stejnou cenu.

Soubor odsoustavy bude obsahovat následující položky:

- $4 fakturace za službu v období od 10. července 9.
- %-3,87 poměrné přeúčtování za službu pro období služby 11. června – 12. června. Toto je období, kdy máte jednu licenci. Výpočet = (měsíční cena/celkový počet dnů v období služby) × dní v poměru periody služby x počet licencí = (4/30) × 29 × 1 = 3,87.
- $7,74 poměrná částka za službu po dobu 12. července 9. Toto je období, kdy byste měli mít dvě licence. Calculation = (4/30) × 29 × 2 = 7,74.

|**Datum nákupu**   |**Začátek platby** |**Konec zpoplatnění**  |**Cena za jednotku**  |**Množství**  |**Částka** |**Typ poplatku** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (máte jednu licenci)     |6/10/2019   |7/09/2019         |$4         |1        |$4            |Nová         |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$3,87       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |4 USD        | 2      |7,74 USD       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Zakoupení předplatného a odebrání licence ve stejný den

Ve scénáři 3 zakoupíte 11. června dvě předplatná pro stejný produkt za jednotkovou cenu 4 USD. Později ve stejný den odeberete jednu z licencí.  

Soubor odsoustavy bude obsahovat následující položky:

- 8 USD se účtuje za dvě licence za období služby od 10. června do 9. července.
- Do 11. června – 11. června přefaktovaná dofakce za službu ve výši 8,00 USD. Jedná se o období, kdy jste měli dvě licence. Výpočet = (měsíční cena / celkové dny v období služby) x dní v přehodnocené době služby × počet licencí = (4/30) x 30 x 2 = 8,00.
- Přefakce 4,00 USD za období služeb od 11. června do 9. července. Jedná se o období, kdy jste měli jednu licenci. Výpočet = (4/30) x 30 x 1 = 4,00.

|**Datum nákupu**   |**Začátek platby** |**Konec zpoplatnění**  |**Cena za jednotku**  |**Množství**  |**Částka** |**Typ poplatku** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |2                 |$8            |Nová         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$8       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 1      |$4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Nákup předplatného a odebrání licencí později

Ve scénáři 4 zakoupíte 11. června dvě předplatná za jednotkovou cenu 4 USD a 12. června odeberete jednu z licencí.

Soubor odsoustavy bude obsahovat následující položky:

- Vyúčtování 8 USD za období služby od 10. června do 9. července.
- 7,74 USD přefakce za období služby 11. až 12. června. Jedná se o období, kdy jste měli dvě licence. Výpočet = (měsíční cena / celkové dny v období služby) × dny v přehodnocené době služby × počet licencí = (4/30) × 29 x 2 = 7,74.
- 3,87 USD přefakce za období služby 12.–9. července Jedná se o období, kdy jste měli jednu licenci. Výpočet = (4/30) x 29 x 1 = 3,87.

|**Datum nákupu**   |**Začátek poplatku** |**Charge end**  |**Jednotková cena**  |**Množství**  |**Částka** |**Typ poplatku** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11. 6. 2019 (máte dvě licence)     |6/10/2019   |7/09/2019         |4 USD         |2        |8 USD       |Nová       |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$7,74       |removeQuantity           |
|6/12/2019 (máte jednu licenci)    | 6/10/2019    |7/09/2019   |$4    |1      |$3,87    |removeQuantity |

## <a name="next-steps"></a>Další kroky

- [Ukázky měsíčních scénářů fakturace pro nové předplatné, změna množství licencí nebo přerušení](common-billing-scenarios-monthly.md)