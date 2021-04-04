---
title: Migrace předplatných Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Edice systém Microsoft Office 365 Enterprise E4 je vyřazení od 7. dubna 2017. Přečtěte si, jak migrovat zákaznická předplatná do novějších verzí Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132617"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrace předplatných Office 365 E4 na novější verze Office 365

**Příslušné role**

- Globální správce
- Správce správy uživatelů
- Agent správce
- Agent prodeje

Plán Office 365 Enterprise E4 je vyřazený, platný 7. dubna 2017. Po tomto datu už nebudete moct koupit nová předplatná Office 365 E4 a existující odběry E4 se po uplynutí této doby nebudou automaticky obnovovat.

Po ukončení předplatných E4 se zruší. Chcete-li zajistit kontinuitu pro zákazníky, měli byste převést zákazníky s vypršením platnosti předplatných E4 na podporovanou možnost SKU, která je uvedena níže. Doporučujeme zákazníkům přesunout nové předplatné před uplynutím ročního koncového data předplatného, aby se předešlo výpadkům služby pro zákazníky. 

> [!NOTE]  
> Vyřadí se SKU komerčních a vládních skladů Office 365 Enterprise E4.
 
Na stránce s podrobnostmi o předplatném se stav předplatného E4 změnil na "vyprší dne [Date]" z "automatické obnovy" v [datum] ". 

Pokud používáte rozhraní API (buď CREST nebo Partnerská centra), můžete zjistit vypršení platnosti předplatného, a to společně s vlastností auto Renew = false. 

Odběry E4 budou nastavené na automatické obnovení = false, 7. dubna 2017. Zákazníky můžete kdykoli přesunout do nového plánu. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Plány nahrazení edice Office 365 Enterprise E4

Můžete se rozhodnout, že budete stejné funkce udržovat s E4, nebo pokud chcete, aby vaši zákazníci využili výhod novějších funkcí a funkcí v Office 365 a Online Skypu pro firmy. Podrobnosti o cenách najdete v seznamu ceníků a v tabulce seznam nabídek v partnerském centru. Zabezpečení produktu Enterprise E3 nebo zabezpečená produktivita Enterprise E5 může být nahrazena následujícími možnostmi pro Office 365 Enterprise E3 nebo Office 365 Enterprise E5.

- Možnost 1: Office 365 Enterprise E5

- Možnost 2: Office 365 Enterprise E3 + Skype pro firmy Cloud PBX

- Možnost 3: Office 365 Enterprise E3 + Skype pro firmy plus CAL (cenová a parita funkčnosti s E4)

- Možnost 4: Office 365 Enterprise E3


| Funkce | Možnost 1 | Možnost 2 | Možnost 3 | Možnost 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Chcete získat všechny funkce zahrnuté v Office 365 Enterprise E4? | Yes | Yes | Yes | No |
| Telefonní čísla spravovaná v sadě Office 365? | Yes | Yes | No | No |
| Telefonní čísla spravovaná místně i v Office 365 (hybridní nasazení)? | Yes | Yes | No | No |
| Možnost přidání plánu hlasového volání veřejné telefonní sítě? | Yes | Yes | No | No |
| Konference v PSTN? | Yes | No | No | No |
| Rozšířené nástroje pro spolupráci, analýzu a zabezpečení? | Yes | No | No | No |
| Interaktivní sestavy, řídicí panely a vizualizace dat? | Yes | No | No | No | 
| Lepší kontrola zabezpečení dat a dodržování předpisů pomocí integrovaných uživatelských ovládacích prvků ochrany osobních údajů, transparentnosti a kontrastu? | Yes | No | No | No | 

## <a name="transition-customers-to-new-product-plans"></a>Přechod zákazníků na nové plány produktů

Microsoft neustále nabízí našim partnerům nové produkty a služby. V těchto případech možná budete muset upgradovat zákazníky na nové služby nebo migrovat své odběry z SKU, které se nakonec vypnou. Migrace zákazníků z vyřazených SKU do novějších vyžaduje následující kroky:

-   Koupit nové předplatné
-   Změna přiřazení licencí k aktuálním uživatelům
-   Zrušit staré předplatné

Pomocí těchto kroků migrujete předplatné Office 365 Enterprise E4 zákazníka na jednu z možností v tabulce výše.

### <a name="step-1---purchase-the-new-subscription"></a>Krok 1 – zakoupení nového předplatného

1. V nabídce **Partnerské centrum** vyberte **zákazníky**, vyberte zákazníka, kterého chcete přesunout, a pak vyberte **Přidat předplatná**.

2. Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat**.

   Váš zákazník by teď měl mít staré i nové předplatné, staré předplatné Office 365 Enterprise E4 a nové předplatné Target, například možnost 1 – Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Krok 2 – Změna přiřazení licencí uživatelům zákazníka

1. V nabídce **Partnerské centrum** vyberte **zákazníky**, vyberte zákazníka, kterého chcete přesunout, a pak vyberte **Uživatelé a licence**. Otevře se stránka uživatelé a licence zákazníka.

2. Pokud chcete změnit přiřazení uživatelských licencí, vyberte uživatele, kterého chcete znovu přiřadit, a pak vyberte **spravovat licence**.

3. Na stránce **spravovat licence** zrušte zaškrtnutí políčka licence **Office 365 Enterprise E4** a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat.

4. Vyberte **Odeslat**. Stránka s potvrzením obsahuje seznam nových přiřazení licencí.

5. Pokračujte stejnými kroky u všech ostatních zákaznických uživatelů, kteří potřebují opětovné přiřazení licence.

Po přesunutí uživatelských licencí do nové služby můžete toto vyřazené předplatné bezpečně zrušit na nejvyšší úrovni zákazníka.

### <a name="step-3---cancel-the-old-subscription"></a>Krok 3 – zrušení původního předplatného

1. V nabídce **Partnerské centrum** vyberte **zákazníci**. Vyberte zákazníka, kterého chcete přesunout, a vyberte předplatné, které chcete zrušit.

2. Na stránce Podrobnosti předplatného nastavte stav předplatného na **pozastaveno**.

3. Vyberte **Odeslat**.

Staré předplatné je pozastavené a nové předplatné je aktivní. Pozastavený odběr bude po 120 dnech automaticky zřízen. Zákazník nevzniká žádné další poplatky za původní předplatné.



 



