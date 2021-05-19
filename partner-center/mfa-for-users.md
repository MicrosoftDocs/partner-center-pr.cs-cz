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
ms.openlocfilehash: 5173526d0f65623311d5cd3a1061e8b9e93e9bb9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151623"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Nastavení vícefaktorového ověřování pro uživatele

**Odpovídající role:** Globální správce

Mezi naše hlavní priority patří větší ochrana osobních údajů a zabezpečení. Víme, že nejlepší obranou je prevence a že jsme jen tak silná jako naše nejslabší propojení. Proto potřebujeme, aby všichni v našem ekosystému jednaly a zajistili, aby byla zajištěna odpovídající ochrana zabezpečení. Důrazně doporučujeme všem partnerům povolit vícefaktorové ověřování (MFA) pro uživatele ve svém partnerském tenantovi. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Přidání vícefaktorového ověřování pro uživatele

Abyste tuto úlohu dokončili, musíte být globálním správcem vaší společnosti.

Je nejjednodušší povolit více ověřování pro uživatele při jejich přidávání do tenanta Azure AD.

1. Přihlaste se [k Azure Portal](https://portal.azure.com) a pak přejděte na **Správa uživatelů.**
1. Vyberte **Multi-Factor Authentication**.
1. Vyberte uživatele, kterého chcete povolit, a pak vyberte **Povolit.**

Tím se pro tohoto uživatele povolí MFA. Povoleno znamená, že při prvním přihlášení se uživateli zobrazí dotaz, jestli má nastavit více ověřování. Následně se při přihlášení zobrazí dotaz, jestli jim pošlete kód, a to buď e-mailem, nebo textovou zprávou (podle toho, které nastavení nastavili).  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Určení způsobu ověření":::

>[!NOTE]
>Pomocí **stejného postupu** jako výše můžete vynutit, aby uživatelé mohli používat MFA, a vybrat **Vynutit**. Další informace najdete v části [Povolení vícefaktorového ověřování Azure pro](/azure/active-directory/authentication/howto-mfa-userstates)uživatele pro zabezpečení událostí přihlášení. 

Všichni uživatelé začínají na **Zakázáno.** Když zaregistrujete uživatele do služby Multi-Factor Authentication Azure Active Directory, jejich stav se změní na **Povoleno.** Když se uživatelé s povoleným přihlášením a dokončí proces registrace, jejich stav se změní na **vynutilo**. 

## <a name="next-steps"></a>Další kroky

- [Přiřazování rolí a oprávnění uživatelům](permissions-overview.md)