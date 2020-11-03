---
title: Postup čtení souboru rekognoskaci vy& účtování
ms.topic: article
ms.date: 06/05/2020
description: Přečtěte si informace o souborech pro odsouhlasení & faktury. Na faktuře se v rámci programu, produktů a zákazníků zobrazí poplatky za partnerské Centrum za toto měsíční období.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: edb2d25b49bd5c40dfd30e9f21d2d8537a5669c4
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/30/2020
ms.locfileid: "92527080"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Seznamte se s fakturací a souborem pro odsouhlasení – Zjistěte, jak je najít v partnerském centru.

**Platí pro**

- Partnerské centrum
- Partnerské centrum pro Microsoft Cloud pro státní správu USA

**Příslušné role**

- Globální správce
- Správce fakturace
- Agent správce


Vaše **Faktura** je **souhrnem všech poplatků za partnerské Centrum** (v rámci programu, všech produktů a všech zákazníků). 

## <a name="invoice-types"></a>Typy faktur

Microsoft bude vydávat jednu fakturu za všechny poplatky založené na licencích (například na Office 365) a poplatky za využití (například Azure) a samostatnou fakturu pro jednorázové poplatky (například Azure CAL, Marketplace nebo plán Azure).

Příklad:  

**Scénář 1 [jediná měna]** : partner má nákupy pro nabídku 145P a licence O365,  

- Partner získá jednu fakturu soubory PDF a 2 odsouhlasení pokrývající poplatky za O365 i Azure (145p).  

**Scénář 2 [jediná měna]** : partner nabízí nákupy pro plán Azure rezervovaných, Marketplace a/nebo Azure společně s nákupy v 145p.

- Partner dostane pro Azure (145p) jednu fakturu a soubor pro odsouhlasení. 

- Partner dostane další fakturační soubory PDF a soubor s odsouhlaskou, který pokrývá poplatky za Azure rezervovaných, Marketplace a plán Azure. 

**Scénář 3 [více měn]** : partner má nákupy pro Azure Ri v DKK a v plánu Azure v eurech společně s 145p nákupy v EUR.

- Partner dostane jeden soubor PDF s fakturací a soubor pro odsouhlasení, který pokrývá poplatky za Azure RI v DKK. 

- Partner dostane v EUR jednu fakturu a soubor pro odsouhlasení zahrnující poplatky za plán Azure. 

- Partner dostane další fakturační PDF a soubor pro odsouhlasení, který pokrývá své poplatky za 145p nabídku v EUR (nebo fakturační měně partnera). 

## <a name="find-your-bill"></a>Hledání faktury 

Fakturu můžete najít na stránce fakturace řídicího panelu v partnerském centru. Na této stránce můžete také najít historii fakturace, trendy útraty a soubory pro odsouhlasení. 

1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/home)partnerského centra. 

2. V nabídce na levé straně vyberte **fakturace** . 

3. Na stránce fakturace vyberte fakturu, kterou chcete stáhnout. 

Odkaz na svou nejnovější fakturu najdete v horní části stránky v části zůstatek účtu k datu poslední faktury. 

Předchozí faktury najdete v části Historie fakturace. Zvolte příslušný rok a potom vyberte šipku rozevíracího seznamu vedle příslušného fakturačního období. Pro stažení faktury této tečky vyberte odkaz vedle faktury (. PDF). 

## <a name="understanding-invoice-pdf"></a>Porozumění formátu PDF faktury 

**Faktury za využití a poplatky na základě licencí** : faktury za poplatky za služby, jako je Office 365 a Azure, budou dostupné do dvou (2) dnů od vybraného fakturačního data [UTC].  

**Faktury za jednorázová a periodické poplatky** : faktury za poplatky za služby, jako je Azure ri, plán Azure, Marketplace budou dostupné až do 8. roku v každém měsíci.  

Níže jsou uvedená některá klíčová pole v dokumentu PDF faktury –

**Číslo faktury** : jedinečný identifikátor dokumentu faktury vygenerovaný pro příslušné fakturační období. 

**Fakturační období** : Toto je období, během kterého máte využití a služby založené na licencích. 

**Datum faktury** : datum fakturace nebo datum výročí, na které se fakturuje každý měsíc. 

**Datum splatnosti platby** : datum, kdy se platba musí přijmout. 

**Poplatky** : částka splatná v fakturační měně pro příslušné fakturační období. 

**Kredity** : kredity (například SLA) nebo úpravy provedené u předplatných (například zvýšení nebo snížení licence). 

**Pokyny pro platbu** : Popis způsobu platby faktury na základě vaší oblasti. Při platbě vždycky nezapomeňte zahrnout číslo vaší faktury. 

Podrobný popis všech polí v souboru faktury (včetně polí pro jednorázové poplatky) naleznete v tématu [pole souboru faktury](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Pochopení souborů pro odsouhlasení

 Soubory pro odsouhlasení, které poskytují podrobné informace o vašich nákladech a jejich podrobnostech, jsou k dispozici ke stažení spolu s PDF faktury. Soubory pro odsouhlasení zahrnují identifikátory zákazníků a identifikátory předplatných, které můžete použít k vytvoření faktur zákazníků. Další informace o souborech rekognoskaci najdete v článku  [Jak používat soubory pro odsouhlasení](use-the-reconciliation-files.md) . 
