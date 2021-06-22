---
title: Nastavení vícefaktorového ověřování pro uživatele
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Zjistěte, jak nastavit zaměstnance pomocí MFA.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9cdb83c8b58b75606275c9773cba79eba75d5d0d
ms.sourcegitcommit: 7cc83714e17337b472727819243f98c84ae181ba
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/22/2021
ms.locfileid: "112450797"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Nastavení vícefaktorového ověřování pro uživatele

**Odpovídající role:** Globální správce

Mezi naše hlavní priority patří větší ochrana osobních údajů a zabezpečení. Víme, že nejlepší obranou je prevence a že jsme jen tak silná jako naše nejslabší propojení. Proto potřebujeme, aby všichni v našem ekosystému jednaly a zajistili odpovídající ochranu zabezpečení. Všem partnerům důrazně doporučujeme povolit vícefaktorové ověřování (MFA) pro své uživatele ve svém partnerském tenantovi. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Přidání vícefaktorového ověřování pro uživatele

Abyste tuto úlohu dokončili, musíte být globálním správcem vaší společnosti.

Je nejjednodušší povolit více ověřování pro uživatele při jejich přidávání do tenanta Azure AD.

1. Přihlaste se [k Azure Portal](https://portal.azure.com) a pak přejděte na **Správa uživatelů.**
1. Vyberte **Multi-Factor Authentication**.
1. Vyberte uživatele, kterého chcete povolit, a pak vyberte **Povolit.**

Tím se pro tohoto uživatele povolí MFA. Povoleno znamená, že při prvním přihlášení se uživateli zobrazí dotaz, jestli má nastavit více ověřování. Následně se při přihlášení zobrazí dotaz, jestli jim má poslat kód, a to buď e-mailem, nebo textovou zprávou (v závislosti na tom, kterou si nastavili).  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="Určete, jak to ověřit.":::

>[!NOTE]
>Pomocí výše **uvedeného** postupu můžete vynutit, aby uživatelé více ověřování mohli používat, a to výběrem **možnosti Vynutit**. Další informace najdete v části [Povolení vícefaktorového](/azure/active-directory/authentication/howto-mfa-userstates)ověřování Azure pro uživatele pro zabezpečení událostí přihlášení. 

Všichni uživatelé začínají na **Zakázáno.** Když zaregistrujete uživatele do služby Multi-Factor Authentication Azure Active Directory, jejich stav se změní na **Povoleno.** Když se uživatelé povolí, přihlásí se a dokončí proces registrace, jejich stav se změní na **Vynucené.** 

## <a name="next-steps"></a>Další kroky

- [Přiřazování rolí a oprávnění uživatelům](permissions-overview.md)