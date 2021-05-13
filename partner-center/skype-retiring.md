---
title: Migrace některých předplatných Skypu pro firmy
description: Zjistěte, jak a kdy migrovat určité zákazníky s vypršeným platnostim předplatných Online Skypu pro firmy Plan 1 na nové verze Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 0e8289ad06dbc8a95f5cff22ca386176d6ba65ab
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854821"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrace předplatných Online Skypu pro firmy (plán 1) na novější verze Office 365

**Odpovídající role:** Agent prodeje

Online Skype for Business Plan 1 bude od 1. srpna 2018 vyřazen z provozu. Po tomto datu už zákazníci nebudou moci kupovat nová předplatná Skypu pro firmy s plánem 1 a stávající předplatná se po vypršení jejich platnosti automaticky neobnoví a neposkytnou možnost prodloužení. Na stránce s podrobnostmi o předplatném se stav předplatného Online Skypu pro firmy (Plán 1) změnil na Platnost vyprší [datum]" z "Automatické prodlužování platnosti k [datum]".  

Pokud chcete zajistit kontinuitu pro zákazníky, měli byste zákazníky s vypršením platnosti předplatných Online Skypu pro firmy ( Plán 1) přeplánovat na podporovanou možnost SKU uvedenou níže. Doporučujeme přestěhovat zákazníky na nová předplatná před ročním datem ukončení předplatného, abyste se vyhnuli výpadkům služeb pro zákazníky. 

>[!NOTE]
>Komerční i státní SKU Skypu pro firmy Online Plán 1 jsou vyřazené z provozu.

Pokud používáte rozhraní API (CREST nebo Partnerské centrum), vyhledejte předplatná, kterým vyprší platnost, vyhodnocením koncového data odběru spolu s vlastností auto renew = False. Předplatná Online Skypu pro firmy Plan 1 se 1. září 2018 nastaví na auto renew=False. Zákazníky můžete kdykoli přesunout do nového plánu. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Náhradní plány online Skypu pro firmy – Plán 1

S novými plány mohou vaši zákazníci využívat novější funkce v Office 365. Podrobnosti o cenách najdete v matici ceníku a seznamu nabídek v Partnerské centrum. 

- Možnost 1: Office 365 Enterprise F1
- Možnost 2: Microsoft 365 Enterprise F1
- Možnost 3: Další plány Office 365

|**Funkce**    |**Možnost 1**   |**Možnost 2**   |**Možnost 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Získejte všechny funkce, které jsou součástí Online Skypu pro firmy – Plán 1.|Yes   |Yes   |Yes   |
|IM a přítomnost |Yes   |Yes   |Yes   |
|Zvuk a video peer-to-peer přes IP adresu|Yes   |Yes   |Yes   
|Připojit schůzky jako ověřeného uživatele| Yes   |Yes   |Yes   |

## <a name="transition-customers-to-new-product-plans"></a>Přechod zákazníků na nové plány produktů

Microsoft neustále nabízí našim partnerům nové produkty a služby. V těchto případech možná budete muset upgradovat zákazníky na nové služby nebo migrovat své odběry z SKU, které se nakonec vypnou. Migrace zákazníků z vyřazených SKU do novějších vyžaduje následující kroky:

- Koupit nové předplatné
- Změna přiřazení licencí k aktuálním uživatelům
- Zrušit staré předplatné

### <a name="migrate-your-customers-to-new-plans"></a>Migrace zákazníků na nové plány

1. Pokud chcete nové předplatné koupit, vyberte v **nabídce partnerské Centrum** možnost **zákazníci**, vyberte zákazníka, kterého chcete přesunout, a pak vyberte **Přidat předplatná**.

2. Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat**. 

Váš zákazník by teď měl mít staré i nové předplatné, staré předplatné online pro Skype pro firmy a nové předplatné Target, třeba možnost 1 – Office 365 Enterprise F1.

3. Pokud chcete znovu přiřadit licence uživatelů zákazníka, vyberte v nabídce **Partnerské centrum** možnost **zákazníci**, vyberte zákazníka, kterého přesouváte, a pak vyberte **Uživatelé a licence**. Otevře se stránka uživatelé a licence zákazníka.

4. Pokud chcete znovu přiřadit uživatelskou licenci, vyberte uživatele, kterého chcete znovu přiřadit, a pak vyberte **spravovat licence.**

5. Na stránce **spravovat licence** zrušte zaškrtnutí políčka licence pro Skype for Business Online Plan 1 a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat.

6. Vyberte **Odeslat**. Stránka s potvrzením obsahuje seznam nových přiřazení licencí. Pokračujte stejným postupem pro ostatní uživatele, kteří potřebují přiřazení licencí.

Po přesunutí uživatelské licence na novou službu můžete vyřazené předplatné bezpečně zrušit na úrovni zákazníka.

7. V **nabídce Partnerské centrum** vyberte **Zákazníci.** Vyberte zákazníka, jehož předplatné zrušíte.

8. Na stránce s podrobnostmi o předplatném nastavte předplatné na **Pozastaveno.**

9. Vyberte **Odeslat.**

Původní předplatné je pozastavené a nové předplatné je aktivní. Pozastavené předplatné bude po 120 dnech automaticky zrušeno. Za staré předplatné se zákazníkovi ne účtuly žádné další poplatky.

## <a name="next-steps"></a>Další kroky

- [Poradci: Vytvoření a odeslání pozvánky ke zkušební verzi pro klienty, kteří si mohou vyzkoušet Office 365](advisors-create-a-trial-invitation.md)
- [Poradci: Vytvoření klientské základny pomocí pozvánek ke zkušební verzi Office 365 a nabídek k nákupu](advisors-build-your-business.md)
- [Poradci: Vytvoření nabídky nákupu](advisor-create-a-purchase-offer.md)
