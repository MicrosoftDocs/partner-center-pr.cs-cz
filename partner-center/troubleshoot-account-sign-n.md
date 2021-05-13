---
title: Řešení potíží s nastavením Partnerské centrum účtu nebo prodloužením platnosti MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Řešení potíží při pokusu o registraci v Partnerské centrum Řeší problémy s způsoby platby, zapomenutím hesel a další.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a5e8a292ad8593dc0b94179d5f0ee418344ef9af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854685"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Řešení potíží s nastavením účtu nebo prodloužením platnosti MPN

**Odpovídající role:** Globální správce | Správce partnera MPN
 
Tady je několik návrhů pro řešení běžných problémů, ke kterým dochází při nastavování Partnerské centrum účtu.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Co se stane, když migrujete z Partner Membership Center a nemůžete upravit žádná pole s informacemi o společnosti

V případech, kdy už vaše společnost existuje v Partnerské centrum (například účet CSP), se zobrazí obrazovka jen pro čtení. Na této obrazovce se zobrazí všechny informace o vaší společnosti, které existují v Partnerské centrum.

Podrobnosti na této obrazovce nemůžete změnit. Jedná se o návrh, a ne o chybu.

Pokračujte **výběrem** možnosti **Přijmout a** Pokračovat.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Pokud oddělení IT vypnulo možnost **Registrace Partnerské centrum**

Tato zpráva se zobrazí, protože virální uživatelé jsou zakázaní nebo je v tenantovi Azure AD zakázaná virální registrace. Globální správce účtu Azure AD může povolit požadované funkce spuštěním následujícího příkazu PowerShellu:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Další informace najdete v [samoobslužné zaregistrovat.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Zapomněli jste své heslo

Pokud jste zapomněli své heslo, vyberte na přihlašovací stránce odkaz Nemáte přístup ke svému účtu?.  Tato možnost umožňuje resetovat heslo nebo požádat globálního správce o přiřazení nových přihlašovacích údajů.

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
