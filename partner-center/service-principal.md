---
title: Objekt služby Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak přidat objekt služby do tenanta Azure AD. To znamená přidání aplikace Azure AD (instančního objektu) do Partnerské centrum.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d12bb66574e6bcee60b2a1df1673dc9171fbee2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854923"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Přidání aplikace Azure AD (instančního objektu) v Partnerské centrum

**Odpovídající role:** Globální správce

V programu komerčního marketplace v Partnerské centrum teď můžete přidat aplikaci Azure AD (instanční objekt) jako uživatele ve vašem Partnerské centrum účtu. (Dříve jste to mohli udělat ve svém portál partnerů cloudu neboli CPP. Teď, když jste migroval do Partnerské centrum, je účet CPP jen pro čtení.)
 
>[!Note] 
>Objekt služby je synonymem pro aplikaci Azure AD.

## <a name="add-an-azure-ad-application-service-principal"></a>Přidání aplikace Azure AD (objekt služby)

1. Na řídicím Partnerské centrum vyberte **Nastavení** a pak vyberte **Nastavení pro vývojáře.**

2. Vyberte **Uživatelé a** pak vyberte Přidat aplikace Azure **AD.**

3. Vyberte existující aplikaci Azure AD nebo vytvořte novou.

4. Pokud vytvoříte novou aplikaci Azure AD, zahrnte následující informace:  

   - **Adresa URL odpovědi:** Adresa URL, na které se uživatelé mohou přihlásit, aby mohli používat vaši aplikaci Azure AD.

   - **Identifikátor URI ID aplikace:** Logický identifikátor aplikace Azure AD, který se zobrazí při odeslání požadavku na jednotné přihlašování do Azure AD.

   - **Role zabezpečení:** Správce rolí **(totéž** jako role Vlastník v CPP) a Vývojář **(totéž** jako role Přispěvatel v CPP) se vztahují na program komerčního marketplace v Partnerské centrum a mohou být přidružené k této aplikaci Azure AD.  

## <a name="next-steps"></a>Další kroky

- [Přehled komerčního marketplace v Partnerské centrum](csp-commercial-marketplace-overview.md)