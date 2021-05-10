---
title: Řešení potíží při nastavování účtu partnerského centra nebo potížích s obnovením MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Řešení potíží při pokusu o registraci v partnerském centru Odpoví na výzvy, které řeší způsoby platby, hesla forgetting a další.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686258"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Řešení potíží s nastavením účtu nebo problémy s obnovením MPN


**Příslušné role**

- Globální správce
- Správce partnera MPN
 
Tady jsou některé návrhy řešení běžných potíží, které vznikají při nastavování účtu partnerského centra.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Co se stane, když migrujete z partnerského centra členství a nemůžete upravovat žádná pole informací o společnosti

V případech, kdy už vaše společnost má přítomnost v partnerském centru (například účet CSP) – zobrazí se obrazovka, která je jen pro čtení. Na této obrazovce se zobrazí všechny informace o vaší společnosti, které v partnerském centru existují.

Podrobnosti na této obrazovce nemůžete změnit. Jedná se o návrh a nejedná se o chybu.

Vyberte **přijmout** a **pokračovat** a pokračujte.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Pokud IT oddělení vypnulo **registraci v partnerském centru**

Tato zpráva se zobrazí, protože virové uživatele jsou zakázané, nebo protože je v tenantovi Azure AD zakázaná registrace viru. Globální správce vašeho účtu Azure AD může povolit požadované funkce spuštěním následujícího příkazu PowerShellu:

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

Další informace najdete v tématu věnovaném [registraci pro samoobslužné služby](/azure/active-directory/users-groups-roles/directory-self-service-signup).

## <a name="you-forgot-your-password"></a>Zapomněli jste heslo

Pokud jste zapomněli heslo, vyberte odkaz **nemáte přístup k účtu?** na přihlašovací stránce. Tato možnost umožňuje resetovat heslo nebo požádat globálního správce o přiřazení nových přihlašovacích údajů.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Na obrazovce Řekněte nám o vaší společnosti se zobrazí chyba Něco se pokazilo

Tato chybová zpráva se obvykle zobrazí, pokud na firemním telefonním čísle neúmyslně použijete speciální znaky, mezery nebo kód země. Hodnota zadaná do pole Telefonní číslo může obsahovat maximálně 10 znaků.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Při nákupu platební karty se zobrazí chybová zpráva s oznámením, že vaše objednávka byla zamítnuta. Ověřte své informace.


Vždy používejte adresu odpovídající vaší platební kartě, a ne právnickou osobu. Také se ujistěte, že je PSČ správné a odpovídá adrese, kterou používáte.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Chcete přepnout z offline platby na online způsob platby 

Budete muset zrušit původní objednávku a znovu ji zakoupit pomocí upřednostňovaného způsobu platby.

Zrušení objednávky:

1. Na **řídicím panelu** vyberte kartu Nabídky členství.

2. Vyberte **Zrušit objednávku.**

3. Zobrazí se potvrzovací okno, které musíte potvrdit, abyste mohli zrušit počáteční objednávku.

## <a name="next-steps"></a>Další kroky

- [Správa účtu v Partnerském centru](partner-center-account-setup.md)
- [Čtení souboru faktury a odsoučtu](read-your-bill.md)
