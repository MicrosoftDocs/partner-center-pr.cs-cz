---
title: Nepovedlo se přihlásit do partnerského centra.
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Řešení možných příčin a získání informací o řešeních, když se nemůžete přihlásit k partnerskému centru – Přečtěte si další informace o resetování hesel, kontrole rolí a kontrole přihlašovacích údajů.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17087727afcaf3dbcf47801f8668388c370758e7
ms.sourcegitcommit: 9b04509f3830462628c1bb6af2ca41ed68b52619
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/09/2021
ms.locfileid: "107266567"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>Řešení potíží s přihlašováním pro partnerské Centrum

**Příslušné role**

- Všichni partneři, kteří mají zájem o partnerské Centrum

Tento článek obsahuje řešení běžných potíží s přihlašováním pro partnerské Centrum.

## <a name="youve-forgotten-your-password-for-partner-center"></a>Zapomněli jste heslo pro partnerské Centrum.

Pokud jste zapomněli heslo a nemůžete se přihlásit do partnerského centra, obraťte se na podporu. Najděte příslušný kontakt na [podporu obchodních produktů](/microsoft-365/admin/contact-support-for-business-products).

Pokud jste partnerem MPN, požádejte svého globálního správce o vytvoření nového hesla. Pokud jste nepřímý prodejce CSP, požádejte svého nepřímý poskytovatel, aby pro vás vytvořil nového globálního správce v tenantovi Azure AD, nebo vytvořte nové heslo za použití jejich delegovaných oprávnění správce.

Pokud chcete získat další informace o tom, jak můžete resetovat heslo a znovu získat přístup k vašemu pracovnímu účtu, přečtěte si téma [resetování svého pracovního nebo školního hesla pomocí bezpečnostních údajů](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>V partnerském centru nemůžete zobrazit ani spravovat očekávané stránky ani možnosti.

Přístup k stránkám v partnerském centru se řídí rolemi, které jste přiřadili. Pokud chcete zjistit, které role jste přiřadili, vyberte v partnerském centru ikonu nastavení, vyberte **Nastavení účtu** a potom v nastavení účtu vyberte **Správa uživatelů**. Do pole Hledat zadejte své jméno a pak zobrazte výsledky.

Pokud nemůžete zobrazit ani spravovat kompetence, zákazníky, pobídky nebo uživatele, které očekáváte, vyzkoušejte následující řešení:

- Pokud chcete získat přístup k funkcím programu MPN, CSP a referenčních seznamů, obraťte se na správce globálního správce nebo účtu. Další informace o rolích a úlohách, které povolují v partnerském centru, najdete v tématu [přiřazení rolí & oprávnění uživatelům](permissions-overview.md).
- Pokud chcete získat přístup k funkcím komerčního tržiště a k Windows & Xbox, Office Storu, Microsoft Edge a vývojářům hardwaru, obraťte se na uživatele v roli vlastníka nebo manažera ve vaší organizaci. Další informace o rolích a oprávněních najdete v tématu [Správa účtu komerčního tržiště v partnerském centru Microsoftu](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>V partnerském centru nemůžete zobrazit vaši nabídku ani výhody

Potvrďte, že k přihlášení používáte správné přihlašovací údaje. Například vaše pracovní a osobní účty můžou vypadat stejně (například abc@contoso.com ), ale jeden z nich může být osobní účet, který jste vytvořili, a další může být nastaven za vás obchodním účtem. V takovém případě, pokud jste přihlášeni, ale nemůžete zobrazit očekávané možnosti týkající se MPN, CSP, komerčního tržiště, zkuste vybrat pracovní účet.

## <a name="next-steps"></a>Další kroky

- [Ověření informací o účtu](verification-responses.md)
- [Resetování hesla](reset-my-pasword.md)
- [Resetování hesla uživatele](reset-a-user-password.md)