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
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151640"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrace Dynamics 365 a plánu Customer Engagement z úrovně Basic na novější verze (u kvalifikovaných nabídek)

**Příslušné role**: globální správce | Správce správy uživatelů | Agent správce | Agent prodeje

Od 1. ledna 2019 zákazníci s Dynamics 365 for Sales/Customing Engagement ze základních (kvalifikovaných nabídek) odběry už nemůžou obnovit tyto starší nabídky. existující odběry se po vypršení platnosti automaticky neobnoví. Na stránce s podrobnostmi o předplatném se stav předplatného změní na "vyprší dne [Date]" z "automatické obnovování v [datum]". 

Chcete-li zajistit kontinuitu pro zákazníky, měli byste je přecházet s vypršením platnosti předplatných na podporovanou možnost, která je uvedena níže. Doporučujeme zákazníkům přesunout nové předplatné před uplynutím ročního koncového data předplatného, aby se předešlo výpadkům služby pro zákazníky.

Pokud používáte rozhraní API (buď CREST nebo Partnerská centra), můžete najít odběry, které vyhodnocuje datum ukončení předplatného spolu s vlastností automaticky obnovit = false. V případě 1. ledna 2019 budou příslušné odběry nastaveny na automatické obnovení = false. Zákazníky můžete kdykoli přesunout do nového plánu. 

### <a name="the-dynamics-365-offers-being-retired"></a>Nabídky Dynamics 365 jsou vyřazeny

- Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka)
- Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro Akademický sbor
- Dynamics 365 pro Sales Enterprise Edition CRMOL Basic (kvalifikovaná nabídka) pro studenty
- Dynamics 365 pro Sales Enterprise Edition (ceny pro státní správu) CRMOL Basic (kvalifikovaná nabídka)
- Dynamics 365 pro Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka)
- Dynamics 365 for Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka) pro Akademický sbor
- Dynamics 365 pro Sales Enterprise Edition od SA pro CRM Basic (kvalifikovaná nabídka) pro studenty
- Dynamics 365 pro Sales Enterprise Edition (ceny pro státní správu) od SA pro CRM Basic (kvalifikovaná nabídka)
- Dynamics 365 for Sales edice Enterprise Add-On for CRM Basic (kvalifikovaná nabídka)
- Dynamics 365 for Sales edice Enterprise Add-On for CRM Basic (kvalifikovaná nabídka) pro učitelské sbory
- Dynamics 365 for Sales edice Enterprise Add-On for CRM Basic (kvalifikovaná nabídka) pro studenty
- Dynamics 365 for Sales edice Enterprise (Ceny pro státní správu) Add-On pro CRM Basic (kvalifikovaná nabídka)
- Plán Dynamics 365 Customer Engagement edice Enterprise CRMOL Basic (kvalifikovaná nabídka)
- Plán Dynamics 365 Customer Engagement edice Enterprise (ceny pro státní správu) CRMOL Basic (kvalifikovaná nabídka)
- Plán Dynamics 365 Customer Engagement edice Enterprise CRMOL Basic (kvalifikovaná nabídka) pro studenty
- Plán Dynamics 365 Customer Engagement edice Enterprise CRMOL Basic (kvalifikovaná nabídka) pro učitelské sbory
- Plán Dynamics 365 Customer Engagement edice Enterprise od SA pro CRM Basic (kvalifikovaná nabídka)
- Plán Dynamics 365 Customer Engagement edice Enterprise (ceny pro státní správu) od SA for CRM Basic (kvalifikovaná nabídka)
- Dynamics 365 Customer Engagement Plan edice Enterprise From SA for CRM Basic (Qualified Offer) for Students
- Plán Dynamics 365 Customer Engagement edice Enterprise od SA pro CRM Basic (kvalifikovaná nabídka) pro učitelské sbory
- Dynamics 365 Customer Engagement Plan edice Enterprise Add-On for CRM Basic (kvalifikovaná nabídka)
- Plán Dynamics 365 Customer Engagement edice Enterprise (ceny pro státní správu) Add-On CRM Basic (kvalifikovaná nabídka)
- Dynamics 365 Customer Engagement Plan edice Enterprise Add-On for CRM Basic (kvalifikovaná nabídka) pro studenty
- Dynamics 365 Customer Engagement Plan edice Enterprise Add-On for CRM Basic (kvalifikovaná nabídka) pro učitelské sbory



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Plán Dynamics 365 for Sales/ Customer Engagement z náhradních plánů Basic (kvalifikované nabídky)

**Vyřazené nabídky**   

- Dynamics 365 for Sales od CRM Basic nebo CRMOL Basic (kvalifikovaná nabídka)
- Plán Dynamics 365 Customer Engagement od CRM Basic nebo CRMOL Basic (kvalifikovaná nabídka)

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
2. Vyberte **přidat odběr**.
3. Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat**. 

Zákazník teď bude mít původní předplatné i nový. Vaším dalším krokem je změna přiřazení licencí uživatelům zákazníka.

1. V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého přesouváte.
2. Vyberte **Uživatelé a licence**.
3. Pokud chcete uživateli přiřadit licenci, vyberte uživatele a pak vyberte **spravovat licence**. 
4. Na stránce **spravovat licence** zrušte zaškrtnutí políčka Dynamics 365 pro možnost plán služby Sales/zákazník Engagement z licence Basic (kvalifikovaná nabídka) a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat. 
5. Vyberte **Odeslat**. To budete dělat pro každého uživatele, který potřebuje novou licenci. 

Po přesunu licencí do nového předplatného můžete staré předplatné zrušit. 

1. V **levém** navigačním panelu vyberte Zákazníci a pak vyberte zákazníka, který přesouváte.
2. Na stránce podrobností o předplatném nastavte staré předplatné na **Pozastaveno** a vyberte **Odeslat.**

Původní předplatné je teď pozastavené a nové předplatné je aktivní. Pozastavené předplatné bude po 120 dnech automaticky zrušeno. Za staré předplatné se zákazníkovi ne účtut žádné další poplatky.
 

 



