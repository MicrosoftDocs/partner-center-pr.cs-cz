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
ms.openlocfilehash: f16b619aba838da1d1da0c5eb13648ebb107c802
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855909"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Seznamte se se souborem vyúčtování a odsouhlasení – zjistěte, jak je najít v Partnerské centrum


**Odpovídající role:** Globální správce | Správce fakturace | Agent pro správu


Vaše **faktura** obsahuje **souhrn všech poplatků za Partnerské centrum** poplatky (v rámci programu, všech produktů a všech zákazníků). 

## <a name="find-your-bill-and-reconciliation-file"></a>Vyhledání vyúčtování a souboru s vyrovnáním 

Fakturu najdete na stránce Fakturace na řídicím panelu v Partnerské centrum. Na této stránce také najdete historii fakturace, trendy útraty a soubory s vyrovnáním. 

1. Přihlaste se k Partnerské centrum [řídicího panelu.](https://partner.microsoft.com/dashboard/home) 

2. V nabídce vlevo vyberte **Fakturace.** 

3. Na stránce stavu fakturace vyberte fakturu nebo soubor vyúčtování, o kterých chcete zobrazit podrobnější informace. 

Odkaz na nejnovější fakturu najdete v horní části stránky v části Zůstatek účtu k datu poslední faktury. 

Předchozí faktury najdete v části Historie fakturace. Zvolte odpovídající rok a pak vyberte šipku rozevíracího seznamu vedle příslušného fakturačního období. Výběrem odkazu vedle možnosti Faktury (.pdf) stáhněte fakturu za toto období. 

## <a name="invoice-types"></a>Typy faktur

Microsoft vydá jednu fakturu za všechny poplatky založené na licencích (například Office 365) a poplatky na základě využití (například Azure) a samostatnou fakturu za poplatky za jednotlivé poplatky (jako je azure RI, Marketplace nebo plán Azure).

Třeba  

**Scénář 1 [Jedna měna]**: Partner má nákupy pro nabídku 145P a licence O365.  

- Partner dostane jednu fakturu ve formátu PDF a 2 soubory s vyrovnáním pokrývající poplatky za O365 i Azure (145p).  

**Scénář 2 [Jedna měna]**: Partneři mají nákupy rezervovaných tržišť Azure, marketplace nebo plánu Azure společně s nákupy s 145 000 000 000 000 000 000 000.

- Partner dostane pro Azure (145p) jednu fakturu a soubor pro odsouhlasení. 

- Partner dostane další fakturační soubory PDF a soubor s odsouhlaskou, který pokrývá poplatky za Azure rezervovaných, Marketplace a plán Azure. 

**Scénář 3 [více měn]**: partner má nákupy pro Azure Ri v DKK a v plánu Azure v eurech společně s 145p nákupy v EUR.

- Partner dostane jeden soubor PDF s fakturací a soubor pro odsouhlasení, který pokrývá poplatky za Azure RI v DKK. 

- Partner dostane v EUR jednu fakturu a soubor pro odsouhlasení zahrnující poplatky za plán Azure. 

- Partner dostane další fakturační PDF a soubor pro odsouhlasení, který pokrývá své poplatky za 145p nabídku v EUR (nebo fakturační měně partnera). 


## <a name="understanding-invoice-pdf"></a>Porozumění formátu PDF faktury 

**Faktury za využití a poplatky na základě licencí**: faktury za poplatky za služby, jako je Office 365 a Azure, budou dostupné do dvou (2) dnů od vybraného fakturačního data [UTC].  

**Faktury za jednorázová a periodické poplatky**: faktury za poplatky za služby, jako je Azure ri, plán Azure, Marketplace budou dostupné až do 8. roku v každém měsíci.  

Níže jsou uvedená některá klíčová pole v dokumentu PDF faktury –

**Číslo faktury**: jedinečný identifikátor dokumentu faktury vygenerovaný pro příslušné fakturační období. 

**Fakturační období**: Toto je období, během kterého máte využití a služby založené na licencích. 

**Datum faktury**: datum fakturace nebo datum výročí, na které se fakturuje každý měsíc. 

**Datum splatnosti platby**: datum, kdy se platba musí přijmout. 

**Poplatky**: částka splatná v fakturační měně pro příslušné fakturační období. 

**Kredity**: kredity (například SLA) nebo úpravy provedené u předplatných (například zvýšení nebo snížení licence). 

**Pokyny pro platbu**: Popis způsobu platby faktury na základě vaší oblasti. Při platbě vždycky nezapomeňte zahrnout číslo vaší faktury. 

Podrobný popis všech polí v souboru faktury (včetně polí pro jednofakturové poplatky) najdete v tématu [Pole souboru faktur.](invoice-file.md) 

## <a name="understand-reconciliation-files"></a>Principy souborů odsouhlasení

 Soubory s vyrovnáním, které poskytují podrobnosti o podrobnostech o poplatcích nebo podrobnostech o položkách, si můžete stáhnout spolu s fakturou PDF. Soubory s vyrovnáním zahrnují identifikátory zákazníků a identifikátory předplatného, které můžete použít k vytváření faktur zákazníků. Další podrobnosti  [o souborech](use-the-reconciliation-files.md) odsouhlasení najdete v tématu Jak používat soubory s vyrovnáním. 

## <a name="next-steps"></a>Další kroky

- [Jak používat soubory s vyrovnáním](use-the-reconciliation-files.md)