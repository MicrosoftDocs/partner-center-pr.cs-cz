---
title: Typy poplatků v souborech s vyrovnáním
ms.topic: article
ms.date: 06/05/2020
description: Seznamte se s typy poplatků (například na základě licencí, na základě využití a jednou), kredity a slevy v Partnerské centrum sesouhlasení.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 10438ba30c6eb5ba5b1daef1ad16521f1f8e77c6
ms.sourcegitcommit: 70b8ebbe0d431c7a13529f9eabd1b24f40108a46
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/14/2021
ms.locfileid: "113989770"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Principy různých typů poplatků v souborech Partnerské centrum odsouhlasení

**Platí pro**: Partnerské centrum | Partnerské centrum pro Microsoft Cloud for US Government

**Odpovídající role:** Agent pro správu | Správce fakturace | Globální správce

Tento článek popisuje mapování mezi oddílem faktury a přidruženými typy poplatků, které můžou být v souboru s vyrovnáním. Na faktuře se zobrazí souhrn poplatků. Soubor s vyrovnáním poskytuje podrobný rozpis transakcí řádkové položky, včetně typů poplatků. Další informace o souborech odsouhlasení najdete v [tématu, jak používat soubory s vyrovnáním.](use-the-reconciliation-files.md)

Jak [soubory s vyrovnáním na](usage-based-recon-files.md) základě využití, tak soubory odsouhlasení na základě licencí zobrazují jenom transakce a poplatky související s využitím (spotřebované jednotky a související poplatky). [](license-based-recon-files.md)

> [!NOTE]
> V souboru s vyrovnáním se nezobrazují nesplacené kredity, slevy nebo refundace, které se zobrazují na faktuře jako vyrovnání. 

## <a name="map-charge-types-to-invoice-charges"></a>Mapování typů poplatků na poplatky za fakturu

Pokud chcete mezi fakturou a souborem s vyrovnáním odkazovat na výše poplatků, použijte možnosti filtrování v Microsoft Excel. Filtrováním podle typů poplatků v souboru s vyrovnáním namapujte poplatky za fakturu na sadu rozpisů poplatků v souboru s vyrovnáním.

## <a name="license-based-charges"></a>Poplatky na základě licencí

Pokud chcete tyto poplatky na základě licencí namapovat na fakturu, sečtete sloupec **Amount** (Částka) ze souboru založeného na licencích.

| Popis poplatku (sloupec ChargeType v souboru s vyrovnáním) | Vysvětlení poplatků |
| ------------------------------------------------------------- | ------------------ |
| Aktivační poplatek | Částka účtované zákazníkovi při použití předplatného po zakoupení. |
| Poplatek za zrušení | Po změně přidružených licencí se zákazníkovi vrátí zaceněné poplatky. |
| Zrušení přenosové rychlosti instancí | Poplatky za předplatná se zruší v případě, že u zákazníka s měsíčním předplatným je předplatné pozastavené a přidružené licence se během stejného měsíce změnily. |
| Poplatek za cyklus | Pravidelné poplatky za předplatné. |
| Cyklické přenosy instancí | Poplatky rozceněné zákazníkem posuzované při změně přidružených licencí. |
| Poplatky za přenos při zrušení | Naceněná refundace za nevyužitou část služby po zrušení. |
| Poplatky za přenos při převodu z aktuální nabídky | Přeceněné poplatky po převodu z aktuálního měsíčního předplatného na roční předplatné. |
| Poplatky za přenos při převodu na novou nabídku | Přehodnocené poplatky po převodu měsíčního předplatného na nové roční předplatné |
| Poplatky za přenos při nákupu | Typ poplatku za předplatné při použití měsíční i roční fakturace. |
| Poplatek za přenos při prodloužení platnosti | Poplatky na základě předplatných při prodloužení platnosti předplatného. |
| Poplatek za prodloužení platnosti | Poplatek za prodloužení platnosti předplatného |
| Poplatky za přenos při aktivaci | Poplatky naceněné od aktivace do konce fakturačního období. |

## <a name="one-time-charges"></a>Poplatky za jeden čas

Pokud chcete tyto jednorázové poplatky namapovat na fakturu, sečtete sloupec **Amount** (Částka) ze souboru založeného na licencích.

| Popis poplatku (sloupec ChargeType v souboru s vyrovnáním) | Vysvětlení poplatků |
| ------------------------------------------------------------- | ------------------ |
| new | Používá se při vytvoření nového nákupu. |
| prodloužení platnosti | Používá se při prodloužení platnosti předplatného po konci tohoto období. |
| addQuantity | Používá se jak u refundace za původní nákup, tak v novém množství po zvýšení. |
| removeQuantity | Používá se jak při refundaci původního nákupu, tak v novém množství po poklesu. |
| cancel (zrušit)Mediate (Náprava) | Používá se při zrušení předplatného. |
| převést | Používá se při upgradu licence. |
| customerCredit | Používá se v případě, že jsou v transakci uvedeny kredity (např. Azure, SLA atd.). |

## <a name="usage-charges"></a>Poplatky za používání

Pokud chcete tyto poplatky za využití namapovat na fakturu, sečtete sloupec **PretaxCharges** ze souboru založeného na využití.

| Popis poplatku (sloupec ChargeType v souboru s vyrovnáním) | Vysvětlení poplatků |
| ------------------------------------------------------------- | ------------------ |
| Vyhodnocení poplatku za využití při zrušení | Přístup k poplatkům za využití při zrušení nezaplaceného využití během aktuálního fakturačního období. |
| Vyhodnocení poplatku za využití pro aktuální cyklus | Přístup k poplatku za využití pro aktuální fakturační období |

### <a name="credits"></a>Kredity

Pokud chcete tyto kredity namapovat na vaši fakturu:

- Sečte **totalForCustomer** ze souboru založeného na licencích.
- Sečte **sloupec PostTaxTotal** ze souboru založeného na využití.

| Popis poplatku (sloupec ChargeType v souboru s vyrovnáním) | Vysvětlení poplatků |
| ------------------------------------------------------------- | ------------------ |
| Posun řádkové položky | Částečná nebo celá refundace řádkové položky, včetně daní. |

### <a name="usage-based-discounts"></a>Slevy založené na využití

Pokud chcete tyto slevy založené na využití namapovat na fakturu, sečtete sloupec **PretaxCharges** ze souboru založeného na využití.

| Popis poplatku (sloupec ChargeType v souboru s vyrovnáním) | Vysvětlení poplatků |
| ------------------------------------------------------------- | ------------------ |
| Sleva za aktivaci | Sleva uplatněná při aktivaci předplatného |
| Sleva za cyklus | Sleva uplatněná na pravidelné poplatky. |
| Sleva za prodloužení platnosti | Sleva uplatněná při prodloužení platnosti předplatného |
| Zrušení slevy | Poplatky uplatněné při zrušení slev |

### <a name="license-based-discounts"></a>Slevy založené na licencích

Pokud chcete na svou fakturu mapovat slevy založené na licencích, sečtete sloupec **TotalOtherDiscount** ze souboru založeného na licencích.

*Slevy založené na licencích je možné uplatnit na více typů poplatků.*
