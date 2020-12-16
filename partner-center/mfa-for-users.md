---
title: Nastavení vícefaktorového ověřování pro uživatele
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Naučte se, jak nastavit vaše zaměstnance na vícefaktorové ověřování.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 355258fd20f867052fa8598e688630005262bb16
ms.sourcegitcommit: ab2ca3c5990b7f920df4ecb9c611d5b1046ec111
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/16/2020
ms.locfileid: "97579974"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Nastavení vícefaktorového ověřování pro uživatele

**Příslušné role**

- Globální správce

Vyšší zabezpečení ochrany osobních údajů a zabezpečení je z našich nejdůležitějších priorit. Víme, že nejlepší obrana je prevence a že máme jenom silný, jako náš slabý odkaz. Proto potřebujeme, aby všichni v našem ekosystému pracovali a zajistili správné fungování ochrany zabezpečení. Všem partnerům důrazně doporučujeme povolit vícefaktorové ověřování (MFA) pro své uživatele v partnerském tenantovi. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Přidání služby Multi-Factor Authentication pro uživatele

Abyste mohli dokončit tuto úlohu, musíte být globálním správcem vaší společnosti.

Je nejjednodušší povolit pro uživatele MFA při jejich přidávání do tenanta Azure AD.

1. Přihlaste se k [Azure Portal](https://portal.azure.com) a pak přejít ke **správě uživatelů**.
1. Vyberte **Multi-Factor Authentication**.
1. Vyberte uživatele, kterého chcete povolit, a pak vyberte **Povolit**.

Tato akce povolí MFA pro tohoto uživatele. Povoleno znamená, že uživatel bude požádán o nastavení ověřování MFA při prvním přihlášení. Po přihlášení se pak vyzve k poskytnutí kódu, který jim pošle e-mailem nebo textovou zprávou (v závislosti na tom, které nastavení).  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Určete, jak se má ověřit":::

>[!NOTE]
>Uživatelům můžete **vyhovět** , aby používali vícefaktorové ověřování pomocí stejných kroků jako výše a **vynutili** výběr. Pokud se chcete dozvědět víc, přečtěte si téma [povolení Multi-Factor Authentication Azure pro jednotlivé uživatele k zabezpečení přihlašovacích událostí](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates). 

Všichni uživatelé začínají **zakázáni**. Když zaregistrujete uživatele v Multi-Factor Authentication Azure pro jednotlivé uživatele, jejich stav se změní na **povoleno**. Když se uživatelé s povoleným přihlášením a dokončí proces registrace, jejich stav se změní na **vynutilo**. 

## <a name="next-steps"></a>Další kroky

- [Přiřazování rolí a oprávnění uživatelům](permissions-overview.md)

