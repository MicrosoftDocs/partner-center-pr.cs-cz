---
title: Čtení souboru s vyúčtováním & odsoustavy
ms.topic: article
ms.date: 06/05/2020
description: Přečtěte si o fakturách a & odsouhlasení. Na vyúčtování se Partnerské centrum poplatky za program, produkty a zákazníky za toto měsíční období.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbdf85d20e15841189191d6b415b54c26378850e
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551193"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Seznamte se se souborem vyúčtování a odsouhlasení – zjistěte, jak je najít v Partnerské centrum


**Odpovídající role:** Globální správce | Správce fakturace | Agent pro správu


Vaše **faktura** obsahuje **souhrn všech poplatků za Partnerské centrum** (v rámci programu, všech produktů a všech zákazníků). 

## <a name="find-your-bill-and-reconciliation-file"></a>Vyhledání souboru vyúčtování a odsouhlasení 

Fakturu najdete na stránce Fakturace na řídicím panelu v Partnerské centrum. Na této stránce také najdete historii fakturace, trendy útraty a soubory s vyrovnáním. 

1. Přihlaste se k řídicímu [Partnerské centrum.](https://partner.microsoft.com/dashboard/home) 

2. V nabídce vlevo vyberte **Fakturace.** 

3. Na stránce stavu fakturace vyberte fakturu nebo soubor vyúčtování, o kterých chcete zobrazit podrobnější informace. 

Odkaz na nejnovější fakturu najdete v horní části stránky v části Zůstatek účtu k datu poslední faktury. 

Předchozí faktury najdete v části Historie fakturace. Zvolte odpovídající rok a pak vyberte šipku rozevíracího seznamu vedle příslušného fakturačního období. Výběrem odkazu vedle možnosti Faktury (.pdf) stáhněte fakturu za toto období. 

## <a name="invoice-types"></a>Typy faktur

Microsoft vydá jednu fakturu za všechny poplatky založené na licencích (například Office 365) a poplatky na základě využití (například Azure) a samostatnou fakturu za poplatky za jednotlivé poplatky (například azure RI, Marketplace nebo plán Azure).

Třeba  

**Scénář 1 [Jedna měna]**: Partner má nákupy pro nabídku 145P a licence Office 365.  

- Partner dostane jednu fakturu ve formátu PDF a dva soubory s vyrovnáním pokrývající poplatky za Office 365 i Azure (145p).  

**Scénář 2 [Jedna měna]**: Partneři mají nákupy rezervovaných tržišť Azure, marketplace nebo plánu Azure společně s nákupy s 145 000 000 000 000 000 000 000.

- Partner dostane jednu fakturu ve formátu PDF a jeden soubor s vyrovnáním, který pokrývá poplatky za Azure (145p). 

- Partner obdrží další fakturu ve formátu PDF a jeden soubor s vyrovnáním, který pokrývá poplatky za rezervované instance (RI) Azure, Marketplace a plán Azure. 

**Scénář 3 [Multi-Currency]**: Partner má nákupy rezervovaných rezervovaných rezervovaných prostředků Azure v podniku VEI, plán Azure v EUR a také nákupy s 145 000 000 000 000 000 000 000 000.

- Partner obdrží jednu fakturu ve formátu PDF a jeden soubor s vyrovnáním, který pokrývá poplatky za ri ri v Azure ve službě FUNKCE. 

- Partner obdrží jednu fakturu ve formátu PDF a jeden soubor s vyrovnáním, který pokrývá poplatky za plán Azure v EUR. 

- Partner obdrží další fakturu ve formátu PDF a jeden soubor s vyrovnáním, který pokrývá poplatky za nabídku 145p v EUR (nebo fakturační měna partnera). 


## <a name="understanding-invoice-pdf"></a>Vysvětlení faktury ve formátu PDF 

**Faktury za poplatky** za využití a licence: Faktury za poplatky za služby jako Office 365 a Azure budou k dispozici do dvou (2) dnů od vybraného fakturačního data [UTC].  

**Faktury za jedno a** opakované poplatky: Faktury za poplatky za služby, jako jsou ri ri azure, plán Azure nebo Marketplace, budou k dispozici nejpozději do 8. dne každého měsíce.  

Níže jsou některá z klíčových polí v dokumentu PDF faktury:

**Číslo faktury:** Jedinečný identifikátor pro fakturovaný dokument vygenerovaný pro příslušné fakturační období. 

**Fakturační období:** Toto je období, během kterého máte využití a služby založené na licencích. 

**Datum faktury:** Fakturační datum nebo datum výročí, kdy se faktura generuje každý měsíc. 

**Datum splatnosti** platby: Datum, do kterého musí být vaše platba přijata. 

**Charges**(Poplatky): Částka splatná ve vaší fakturační měně pro příslušné fakturační období. 

**Kredity:** Kredity (například smlouvy o úrovni služeb (SLA)) nebo úpravy změn provedených v předplatných (například zvýšení nebo snížení licencí). 

**Pokyny k** platbě: Popis způsobu úhrady faktury v závislosti na vaší oblasti. Při provádění platby vždy nezapomeňte zahrnovat číslo faktury. 

Podrobný popis všech polí v souboru faktury (včetně polí pro jednofakturové poplatky) najdete v tématu [Pole souboru faktur.](invoice-file.md) 

## <a name="understand-reconciliation-files"></a>Principy souborů odsouhlasení

 Soubory s vyrovnáním, které poskytují podrobnosti o vašich poplatcích v podrobnostech nebo položkách, si můžete stáhnout spolu s fakturou PDF. Soubory s vyrovnáním zahrnují identifikátory zákazníků a identifikátory předplatného, které můžete použít k vytváření faktur zákazníků. Další informace o souborech odsouhlasení najdete v [tématu Jak používat soubory s vyrovnáním.](use-the-reconciliation-files.md) 

## <a name="next-steps"></a>Další kroky

- [Jak používat soubory s vyrovnáním](use-the-reconciliation-files.md)