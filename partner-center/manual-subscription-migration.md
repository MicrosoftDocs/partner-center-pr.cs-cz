---
title: Migrace úplných předplatných Dynamics 365
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak migrovat z kvalifikovaných předplatných, Basic Dynamics 365 na nové předplatné dřív, než vyprší platnost stávajících předplatných.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8575d87ab3c4c7970135a87b7ef7564c4fe06232
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/17/2020
ms.locfileid: "92527031"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrace Dynamics 365 a plánu Customer Engagement z úrovně Basic na novější verze (u kvalifikovaných nabídek)

**Platí pro**

-  Partnerské centrum

**Příslušné role**
-   Globální správce
-   Správce uživatelů
-   Agent správce
-   Agent prodeje

Od 1. ledna 2019 zákazníci s Dynamics 365 for Sales/Customing Engagement ze základních (kvalifikovaných nabídek) odběry už nemůžou obnovit tyto starší nabídky. existující odběry se po vypršení platnosti automaticky neobnoví. Na stránce s podrobnostmi o předplatném se stav předplatného změní na "vyprší dne [Date]" z "automatické obnovování v [datum]". 

Chcete-li zajistit kontinuitu pro zákazníky, měli byste je přecházet s vypršením platnosti předplatných na podporovanou možnost, která je uvedena níže. Doporučujeme zákazníkům přesunout nové předplatné před uplynutím ročního koncového data předplatného, aby se předešlo výpadkům služby pro zákazníky.

Pokud používáte rozhraní API (buď CREST nebo Partnerská centra), můžete najít odběry, které vyhodnocuje datum ukončení předplatného spolu s vlastností automaticky obnovit = false. V případě 1. ledna 2019 budou předplatná nastavena na hodnotu automaticky obnovit = false. Zákazníky můžete kdykoli přesunout do nového plánu. 

### <a name="the-dynamics-365-offers-being-retired"></a>Nabídky Dynamics 365 jsou vyřazeny

- Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka)
- Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro Akademický sbor
- Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro studenty
- Dynamics 365 pro Sales Enterprise Edition (ceny pro státní správu) CRMOL Basic (kvalifikovaná nabídka)
- Dynamics 365 pro Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka)
- Dynamics 365 for Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka) pro Akademický sbor
- Dynamics 365 pro Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka) pro studenty
- Dynamics 365 pro Sales Enterprise Edition (ceny pro státní správu) od SA pro CRM Basic (kvalifikovaná nabídka)
- Dynamics 365 pro Sales Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka)
- Dynamics 365 pro prodej Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka) pro Akademický sbor
- Dynamics 365 pro prodej Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka) pro studenty
- Dynamics 365 pro Sales Enterprise Edition (ceny pro státní správu) Add-On pro CRM Basic (kvalifikovaná nabídka)
- Dynamics 365 Customer Engagement plán Enterprise Edition CRMOL úrovně Basic (kvalifikovaná nabídka)
- Dynamics 365 Customer Engagement Enterprise Edition (ceny pro státní správu) CRMOL Basic (kvalifikovaná nabídka)
- Dynamics 365 Customer Engagement plán Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro studenty
- Dynamics 365 Customer Engagement plán Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro Akademický sbor
- Dynamics 365 Customer Engagement plán Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka)
- Dynamics 365 Customer Engagement plán Enterprise Edition (ceny pro státní správu) od SA pro CRM Basic (kvalifikovaná nabídka)
- Dynamics 365 Customer Engagement plán Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka) pro studenty
- Dynamics 365 Customer Engagement plán Enterprise Edition od společnosti SA pro aplikaci CRM Basic (kvalifikovaná nabídka) pro Akademický sbor
- Dynamics 365 Customer Engagement – Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka)
- Dynamics 365 Customer Engagement plán Enterprise Edition (ceny pro státní správu) Add-On pro CRM Basic (kvalifikovaná nabídka)
- Dynamics 365 Customer Engagement pro zákazníky – edice Enterprise Add-On pro CRM Basic (kvalifikovaná nabídka) pro studenty
- Dynamics 365 Customer Engagement – Enterprise Edition Add-On pro CRM Basic (kvalifikovaná nabídka) pro Akademický sbor



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 pro plánování služby Sales/Customer Engagement ze základních (kvalifikovaných nabídek) plánů nahrazení

**Vyřazené nabídky**   

- Dynamics 365 pro prodej z aplikace CRM Basic nebo CRMOL Basic (kvalifikovaná nabídka)
- Plán Customer Engagement pro Dynamics 365 od CRM Basic nebo CRMOL Basic (kvalifikovaná nabídka)

**Možnosti nahrazení**
- Dynamics 365 pro prodejní specialisty (nové)
- Dynamics 365 pro prodejní specialisty (nové)
- Dynamics 365 for Customer Service
- Plán Customer Engagement pro Dynamics 365 nebo
- Členové týmu Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Přechod zákazníků na nové plány produktů

Přesun zákazníků z vyřazených SKU do novějšího vyžaduje následující kroky v tomto pořadí:

- Koupit nové předplatné
- Změna přiřazení licencí k aktuálním uživatelům
- Zrušit staré předplatné

## <a name="purchase-the-new-plan-for-your-customer"></a>Zakupte si nový plán pro zákazníka.

1. V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého chcete přesunout do nového předplatného.
2. Vyberte **přidat odběr** .
3. Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat** . 

Zákazník teď bude mít původní předplatné i nový. Vaším dalším krokem je změna přiřazení licencí uživatelům zákazníka.

1. V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého přesouváte.
2. Vyberte **Uživatelé a licence** .
3. Pokud chcete uživateli přiřadit licenci, vyberte uživatele a pak vyberte **spravovat licence** . 
4. Na stránce **spravovat licence** zrušte zaškrtnutí políčka Dynamics 365 pro možnost plán služby Sales/zákazník Engagement z licence Basic (kvalifikovaná nabídka) a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat. 
5. Vyberte **Odeslat** . To provedete pro každého uživatele, který bude tuto novou licenci potřebovat. 

Po přesunutí licencí do nového předplatného můžete zrušit původní předplatné. 

1. V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého přesouváte.
2. Na stránce s podrobnostmi předplatného nastavte původní předplatné na **pozastaveno** a vyberte **Odeslat** .

Staré předplatné je teď pozastavené a nové předplatné je aktivní. Pozastavený odběr bude po 120 dnech automaticky zřízen. Pro staré předplatné nepřijde váš zákazník žádné další poplatky.
 

 



