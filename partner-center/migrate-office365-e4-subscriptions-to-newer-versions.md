---
title: Migrace předplatných Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: systém Microsoft Office 365 Enterprise E4 se k 7. dubnu 2017 vyřazena. Zjistěte, jak migrovat předplatná zákazníků na novější verze Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f738ddace805838cdf202c23cca8535c11cbdf54
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151555"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrace předplatných Office 365 E4 na novější verze Office 365

**Odpovídající role:** Globální správce | Správce správy uživatelů | Agent správy | Agent prodeje

Plán Office 365 Enterprise E4 je od 7. dubna 2017 vyřazený. Po tomto datu už není možné kupovat nová předplatná Office 365 E4 a stávající předplatná E4 se po vypršení jejich platnosti automaticky neobnoví.

Po skončení předplatných E4 se zruší. Pokud chcete zajistit kontinuitu pro zákazníky, měli byste zákazníky s předplatným E4 s vypršenou platnosti pře převodem na podporovanou možnost SKU uvedenou níže. Doporučujeme přestěhovat zákazníky na nová předplatná před ročním datem ukončení předplatného, abyste se vyhnuli výpadkům služeb pro zákazníky. 

> [!NOTE]  
> Komerční i státní SKU Office 365 Enterprise E4 jsou vyřazené z provozu.
 
Na stránce s podrobnostmi o předplatném se stav předplatného E4 změnil na Platnost vyprší [datum]" z "Automatické prodloužení platnosti k [datum]". 

Pokud používáte rozhraní API (CREST nebo Partnerské centrum), můžete zjistit předplatná, kterým vyprší platnost, vyhodnocením koncového data odběru spolu s vlastností auto renew = False. 

V 7. dubnu 2017 se předplatná E4 nastaví na auto renew=False. Zákazníky můžete kdykoli přesunout do nového plánu. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Plány nahrazení edice Office 365 Enterprise E4

Můžete se rozhodnout pro zachování stejných funkcí s E4 nebo můžete svým zákazníkům využít novější funkce v Office 365 a Online Skypu pro firmy. Podrobnosti o cenách najdete v matici ceníku a seznamu nabídek v Partnerské centrum. Možnost Secure Product Enterprise E3 nebo Secure Productive Enterprise E5 může být nahrazena následujícími možnostmi pro Office 365 Enterprise E3 nebo Office 365 Enterprise E5.

- Možnost 1: Office 365 Enterprise E5

- Možnost 2: Soubor PBX Office 365 Enterprise E3 + Skype pro firmy

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

### <a name="step-1---purchase-the-new-subscription"></a>Krok 1 – Zakoupení nového předplatného

1. V **Partnerské centrum** vyberte **Zákazníci,** vyberte zákazníka, který chcete přesunout, a pak vyberte **Přidat předplatná**.

2. Vyberte předplatné, které chcete zakoupit z katalogu (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat.**

   Váš zákazník by teď měl mít stará i nová předplatná, staré předplatné Office 365 Enterprise E4 a nové cílové předplatné, například možnost 1 – Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Krok 2 – Opětovné přiřazení licencí uživatelů zákazníka

1. V **Partnerské centrum** vyberte **Zákazníci,** vyberte zákazníka, který chcete přesunout, a pak vyberte **Uživatelé a licence.** Otevře se stránka Uživatelé a licence zákazníka.

2. Pokud chcete znovu přiřadit uživatelské licence, vyberte uživatele, který chcete znovu přiřadit, a pak vyberte **Spravovat licence.**

3. Na stránce **Spravovat licence** zrušte zaškrtnutí políčka Licence **Office 365 Enterprise E4** a vyberte nový plán služby pro předplatné, do které zákazník přesouvá.

4. Vyberte **Odeslat**. Na potvrzovací stránce se zobrazí nová přiřazení licencí.

5. Pokračujte ve stejných krocích u všech ostatních zákaznických uživatelů, kteří potřebují znovu přiřadit licenci.

Po přesunutí uživatelských licencí do nové služby můžete vyřazené předplatné bezpečně zrušit na nejvyšší úrovni zákazníka.

### <a name="step-3---cancel-the-old-subscription"></a>Krok 3 – Zrušení starého předplatného

1. V **nabídce Partnerské centrum** vyberte **Zákazníci.** Vyberte zákazníka, kterého chcete přesunout, a vyberte předplatné, které chcete zrušit.

2. Na stránce s podrobnostmi o předplatném nastavte stav předplatného na **Pozastaveno.**

3. Vyberte **Odeslat**.

Původní předplatné je pozastavené a nové předplatné je aktivní. Pozastavené předplatné bude po 120 dnech automaticky zrušeno. Za staré předplatné se zákazníkovi ne účtuly žádné další poplatky.



 



