---
title: Výpočet efektivní jednotkové ceny
ms.topic: how-to
ms.date: 04/02/2021
description: Přečtěte si o efektivní jednotkové ceně a o tom, jak se počítá. Tento článek obsahuje také ukázkový výpočet.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147118"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Výpočet efektivní jednotkové ceny pro spotřebu plánu Azure

**Odpovídající role:** Správce fakturace

## <a name="the-effective-unit-price"></a>Efektivní jednotková cena

Efektivní jednotková cena se počítá na úrovni měřiče (na rozdíl od úrovně prostředků) a každý den se upravuje podle využití měřiče.

Efektivní jednotkovou cenu vypočítáme pomocí následujících tří faktorů:

- Spotřeba, která se monitoruje každý den v průběhu fakturačního cyklu
- Fakturovatelné náklady na měřič
- Vrstvení (pokud je to dostupné)

Vzhledem k tomu, že spotřebu sledujeme každý den v průběhu fakturačního cyklu, bude efektivní jednotková cena kolísá. Konečná cena za dané fakturační období bude k dispozici po zastavení výpočtu spotřeby a uzavření fakturačního období. Většinu změn spotřeby uvidíte po čtvrtém nebo pátém desetinném místě.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Zjistěte, jestli váš měřič používá vrstvené ceny.

Pokud nevíte, jestli váš měřič používá vrstvené ceny, zjistěte to pomocí následujícího postupu. 

1. Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).
2. Vyberte **Sell (Prodej),** **vyberte Pricing and offers (Ceny** a nabídky) a pak vyberte **Azure Plan pricing (Ceny plánu Azure).**
3. Vyhledejte měřič podle ID a stáhněte si data o cenách. 

## <a name="sample-calculation"></a>Ukázkový výpočet

Následující tabulka uvádí příklad, jak vypočítáme efektivní jednotkovou cenu během otevřeného období.

V tabulce platí následující hodnoty: 

- **UP** = jednotková cena prostředku za hodinu = 0,868

- **BCU** = fakturovatelná jednotka spotřeby měřiče

- **BC** = fakturovatelné náklady na měřič = BCU * UP * 0,85. To odráží úpravu pro 15% slevu PEC. Potom použijeme dolní limit funkce k omezení hodnoty na dvě číslice za desetinnou čárkou, aby bylo možné účtovat minimální částku. 

- **Efektivní jednotková cena** = BCU/BC

>[!NOTE]

>Poznámka: Měřič v tomto příkladu nemá úrovně v cenách ani jiných slevách – efektivní jednotková cena bere v úvahu procentuální slevy a další úpravy.


| Date (Datum) | BCU (fakturovatelná jednotka spotřeby) | BC (fakturovatelné náklady) | Efektivní jednotková cena |
| ------ | ----------- | ----------- | ----------- |  
| 3.8. | 29 | 21.39 | 0.737586206896552 |
| 10. srpna | 210.950039 | 155.63 | 0.737757626107858 |
| 25. srpna | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>Další kroky

- [Fakturace a daně](billing.md)
