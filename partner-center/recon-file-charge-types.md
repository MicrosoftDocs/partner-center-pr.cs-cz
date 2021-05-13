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
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855875"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Pochopení různých typů poplatků v souborech pro odsouhlasení partnerského centra

**Platí pro**: partnerské Centrum | Partnerské centrum pro Microsoft Cloud pro státní správu USA

**Příslušné role**: Agent správce | Správce fakturace | Globální správce

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
| Zrušit poplatek | Po změně přidružených licencí se zákazníkovi vrátí zaceněné poplatky. |
| Zrušení přenosové rychlosti instancí | Poplatky za předplatná se zruší v případě, že u zákazníka s měsíčním předplatným je předplatné pozastavené a přidružené licence se během stejného měsíce změnily. |
| Poplatek za cyklus | Pravidelné poplatky za předplatné. |
| Cyklické přenosy instancí | Poplatky rozceněné zákazníkem posuzované při změně přidružených licencí. |
| Poplatky za přenos při zrušení | Naceněná refundace za nevyužitou část služby po zrušení. |
| Poplatky za přenos při převodu z aktuální nabídky | Přeceněné poplatky po převodu z aktuálního měsíčního předplatného na roční předplatné. |
| Poplatky za přenos při převodu na novou nabídku | Přehodnocené poplatky po převodu měsíčního předplatného na nové roční předplatné. |
| Poplatky za přenos při nákupu | Typ poplatku za předplatné při použití měsíční i roční fakturace. |
| Poplatek za přenos při prodloužení platnosti | Poplatky na základě předplatných při prodloužení platnosti předplatného. |
| Poplatek za prodloužení platnosti | Poplatek za prodloužení platnosti předplatného |
| Poplatky za přenos při aktivaci | Poměrné poplatky od aktivace až do konce fakturačního období. |

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

*Slevy založené na licencích mohou být uplatněny na více typů poplatků.*
