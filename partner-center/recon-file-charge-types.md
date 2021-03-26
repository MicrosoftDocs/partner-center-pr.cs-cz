---
title: Typy poplatků v souborech s vyrovnáním
ms.topic: article
ms.date: 06/05/2020
description: Seznamte se s typy poplatků (jako jsou založené na licencích a na základě využití a jednorázové), kredity a slevy v souborech pro odsouhlasení partnerského centra.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ba42ac5beb28a3cf819c54a86385fb79853cdcd0
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549222"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Pochopení různých typů poplatků v souborech pro odsouhlasení partnerského centra

**Platí pro**

- Partnerské centrum pro oficiální Cloud Microsoftu

**Příslušné role**

- Agent správce
- Správce fakturace
- Globální správce

Tento článek popisuje mapování mezi oddílem faktury a typy přidružených poplatků, které mohou být na vašem souboru pro odsouhlasení. Vaše faktura poskytuje souhrn poplatků. Váš soubor pro odsouhlasení poskytuje podrobný rozpis transakcí položek řádků, včetně typů poplatků. Další informace o souborech pro odsouhlasení najdete v tématu [Jak používat soubory pro odsouhlasení](use-the-reconciliation-files.md).

[Soubory odsouhlasení založené na použití](usage-based-recon-files.md) a [soubory odsouhlasení založené na licencích](license-based-recon-files.md) zobrazují jenom transakce a poplatky související s využitím (spotřebované jednotky a související poplatky).

> [!NOTE]
> Jednorázové kredity, slevy nebo refundace, které se zobrazí na faktuře jako **Úpravy** , se v souboru pro odsouhlasení nezobrazují.

## <a name="map-charge-types-to-invoice-charges"></a>Mapování typů nákladů na faktury

Chcete-li náklady na křížové odkazy mezi vaším souborem faktury a odsouhlasení, použijte možnosti filtru v aplikaci Microsoft Excel. Filtrovat poplatky za fakturu na sadu rozdělení poplatků v souboru odsouhlasení podle typu poplatků za poplatek.

## <a name="license-based-charges"></a>Poplatky na základě licencí

Chcete-li namapovat tyto poplatky na základě licencí na fakturu, sečtěte sloupec **částky** ze souboru založeného na licencích.

| Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení) | Vysvětlení poplatků |
| ------------------------------------------------------------- | ------------------ |
| Aktivační poplatek | Částka, která se účtuje zákazníkovi při použití předplatného po nákupu |
| Zrušit poplatek | Poměrné náklady se účtují zákazníkovi při změně přidružených licencí. |
| Zrušit poměr instancí | Poměrné poplatky se zrušily, když zákazník s měsíčním předplatným má předplatné pozastaveno a přidružené licence se v rámci stejného měsíce změnily. |
| Poplatek za cyklus | Pravidelné poplatky za předplatné |
| Poměr instance cyklu | Poměrné poplatky se od zákazníka vyhodnotily při změně přidružených licencí. |
| Poměr poplatků při zrušení | Poměrná refundace nevyužité části služby při zrušení. |
| Poměrné poplatky při převodu z aktuální nabídky | Poměrné náklady po převodu od aktuálního měsíčního předplatného na roční předplatné |
| Poměrné poplatky při převodu na novou nabídku | Poměrné náklady po převodu měsíčního předplatného na nové roční předplatné. |
| Poměrné poplatky při nákupu | Typ poplatků pro předplatné při použití měsíčního nebo ročního účtování. |
| Poplatek za prodlužování | Poměrné poplatky při obnovení předplatného. |
| Prodloužit poplatek | Poplatek za obnovení předplatného |
| Poplatky za rychlost při aktivaci | Poměrné poplatky od aktivace až do konce fakturačního období. |

## <a name="one-time-charges"></a>Jednorázové poplatky

Chcete-li namapovat tyto jednorázové poplatky na fakturu, sečtěte sloupec **částky** ze souboru založeného na licencích.

| Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení) | Vysvětlení poplatků |
| ------------------------------------------------------------- | ------------------ |
| Nová | Používá se při vytvoření nového nákupu. |
| addQuantity | Používá se v refundaci původního nákupu i v novém množství po zvýšení. |
| removeQuantity | Používá se v refundaci původního nákupu i v novém množství po zmenšení. |
| Zrušit | Používá se při zrušení odběru. |
| Převést | Používá se při upgradu licence, ale počet licencí zůstane beze změny. |

## <a name="usage-charges"></a>Poplatky za používání

Pokud chcete namapovat tyto poplatky za použití na fakturu, sečtěte sloupec **PretaxCharges** ze souboru založeného na využití.

| Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení) | Vysvětlení poplatků |
| ------------------------------------------------------------- | ------------------ |
| Vyhodnotit poplatek za použití při zrušení | Použít poplatek za použití při zrušení neplaceného využití během aktuálního fakturačního období. |
| Vyhodnotit poplatek za použití pro aktuální cyklus | Přístup k poplatku za použití pro aktuální fakturační období |

### <a name="credits"></a>Kredity

Chcete-li namapovat tyto kredity na vaši fakturu:

- Sečtěte **TotalForCustomer** ze souboru založeného na licencích.
- Sečtěte sloupec **PostTaxTotal** ze souboru založeného na využití.

| Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení) | Vysvětlení poplatků |
| ------------------------------------------------------------- | ------------------ |
| Posunutí položky řádku | Částečná nebo celá náhrada za položku na řádku, včetně daní. |

### <a name="usage-based-discounts"></a>Slevy na základě využití

Pokud chcete tyto slevy na základě využití namapovat na fakturu, sečtěte sloupec **PretaxCharges** ze souboru založeného na využití.

| Popis poplatku (sloupec ChargeType v souboru pro odsouhlasení) | Vysvětlení poplatků |
| ------------------------------------------------------------- | ------------------ |
| Aktivační sleva | Sleva použitá při aktivaci předplatného |
| Sleva na cyklus | Zvýhodněná sleva se účtuje na základě pravidelných poplatků. |
| Prodloužit slevu | Sleva použitá při obnovení předplatného |
| Zrušit slevu | Poplatky se účtují při zrušení slev. |

### <a name="license-based-discounts"></a>Slevy na základě licencí

Chcete-li namapovat slevy na základě licencí na fakturu, sečtěte sloupec **TotalOtherDiscount** ze souboru založeného na licencích.

*Slevy založené na licencích mohou být uplatněny na více typů poplatků.*
