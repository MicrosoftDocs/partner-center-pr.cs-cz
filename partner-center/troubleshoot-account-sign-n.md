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
ms.openlocfilehash: 9622f02039360e8ab39f459c9a2fe082ec70c854
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756739"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Řešení potíží s nastavením účtu nebo problémy s obnovením MPN


**Příslušné role**

- Globální správce
- Správce partnera MPN 
 
Tady jsou některé návrhy řešení běžných potíží, které vznikají při nastavování účtu partnerského centra.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Co se stane, když migrujete z partnerského centra členství a nemůžete upravovat žádná pole informací o společnosti

V případech, kdy už vaše společnost má přítomnost v partnerském centru (Řekněte mu účet CSP) – zobrazí se obrazovka, která je jen pro čtení. Na této obrazovce se zobrazí všechny informace o vaší společnosti, které v partnerském centru existují.

Podrobnosti na této obrazovce nemůžete změnit. Jedná se o návrh a nejedná se o chybu.

Vyberte **přijmout** a **pokračovat** a pokračujte.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Pokud IT oddělení vypnulo **registraci v partnerském centru**.

Tato zpráva se zobrazí, protože virové uživatele jsou zakázané, nebo protože je v tenantovi Azure AD zakázaná registrace viru. Globální správce vašeho účtu Azure AD může povolit požadované funkce spuštěním následujícího příkazu PowerShellu:

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

Další informace najdete v tématu věnovaném [registraci samoobslužných služeb](/azure/active-directory/users-groups-roles/directory-self-service-signup) .

## <a name="you-forgot-your-password"></a>Zapomněli jste heslo

Pokud jste zapomněli heslo, vyberte odkaz **nemáte přístup k účtu?** na přihlašovací stránce. Tato možnost umožňuje resetovat heslo nebo požádat globálního správce, aby vám přiřadil nové přihlašovací údaje.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Na obrazovce řekněte nám o vaší firmě se zobrazí chyba "něco se pokazilo".

Tato chybová zpráva se obvykle zobrazuje, pokud nechtěně používáte v telefonním čísle vaší společnosti speciální znaky, mezery nebo kód země. Hodnota zadaná v poli telefonní číslo může obsahovat jenom maximálně 10 znaků.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Nákup vaší platební karty obdržíte chybovou zprávu s oznámením, že vaše objednávka byla zamítnuta. Ověřte prosím vaše informace.


Vždy používejte adresu odpovídající vaší kreditní kartě, nikoli vaší právní entitu. Také se ujistěte, že je poštovní směrovací číslo správné a odpovídá adrese, kterou používáte.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Chcete přepnout z offline platby na online způsob platby 

Původní objednávku bude nutné zrušit a znovu zakoupit pomocí preferovaného způsobu platby.

Postup zrušení objednávky:

1. Na řídicím panelu vyberte kartu **nabídky členství** .

2. Vyberte možnost **zrušit pořadí** .

3. Zobrazí se potvrzovací okno, které je nutné potvrdit, aby bylo možné původní pořadí zrušit.

## <a name="next-steps"></a>Další kroky

- [Správa účtu v Partnerském centru](partner-center-account-setup.md)
- [Jak číst váš soubor fakturace a rekognoskaci](read-your-bill.md)
