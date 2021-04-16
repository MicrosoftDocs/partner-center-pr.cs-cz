---
title: Výpočet efektivní jednotkové ceny
ms.topic: how-to
ms.date: 04/02/2021
description: Přečtěte si o efektivní jednotkové ceně a způsobu jejich výpočtu. Tento článek obsahuje také ukázkový výpočet.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6c3c3a672de015c9f38fa0e34232da8d9913177c
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528568"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Efektivní výpočet jednotkové ceny pro spotřebu plánu Azure

## <a name="the-effective-unit-price"></a>Efektivní Jednotková cena

Platná Jednotková cena se vypočítá na úrovni měřiče (na rozdíl od úrovně prostředku) a v závislosti na využití měřiče se upraví každý den.

Platnou jednotkovou cenu vypočítáme pomocí následujících tří faktorů:

- Spotřeba, která se denně monitoruje v průběhu fakturačního cyklu
- Fakturovatelné náklady za měřič
- Vrstvení (Pokud je k dispozici)

Vzhledem k tomu, že monitoruje denní spotřebu v průběhu fakturačního cyklu, efektivní Jednotková cena bude kolísat. Konečná cena za daný fakturační cyklus bude k dispozici po zastavení výpočtu spotřeby a uzavření fakturačního období. Po čtvrtém nebo pátém desetinném místě uvidíte většinu změn v spotřebě.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Zjistěte, jestli měřič používá vrstvené ceny.

Pokud si nejste jistí, jestli měřič používá vrstvené ceny, najděte pomocí níže uvedeného postupu. 

1. Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).
2. Vyberte **prodávat**, vyberte **ceny a nabídky** a pak vyberte **ceny plánu Azure**.
3. Vyhledejte měřič podle ID a Stáhněte si data o cenách. 

## <a name="sample-calculation"></a>Ukázkový výpočet

V následující tabulce najdete příklad toho, jak vypočítat efektivní jednotkovou cenu během otevřeného období.

V tabulce platí následující hodnoty: 

- **Nahoru** = Jednotková cena prostředku/hodiny = 0,868

- **BCU** = fakturovatelná jednotka spotřeby pro měřič

- **BC** = Fakturovatelné náklady za měřič = BCU * nahoru × 0,85. To odráží úpravu pro 15% slevu PEC. Pak použijeme spodní limit funkce k omezení hodnoty na dvě číslice za desetinnou čárkou, aby se využívala minimální částka. 

- **Efektivní Jednotková cena** = BCU/BC

>[!NOTE]

>Poznámka: měřič v tomto příkladu nemá úrovně v cenách nebo jiných slevách – efektivní faktory pro ceny za jednotku v procentech slevy a další úpravy.


| Date (Datum) | BCU (jednotka fakturovatelných spotřeby) | BC (Fakturovatelné náklady) | Efektivní Jednotková cena |
| ------ | ----------- | ----------- | ----------- |  
| 3. srpna | 29 | 21,39 | 0.737586206896552 |
| 10. srpna | 210,950039 | 155,63 | 0.737757626107858 |
| 25. srpna | 555,950039 | 410,17 | 0.737782122900436 |

## <a name="next-steps"></a>Další kroky

- [Fakturace a daně](billing.md)
