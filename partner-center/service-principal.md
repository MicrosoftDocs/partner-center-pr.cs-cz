---
title: Instanční objekt služby Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak přidat instanční objekt k vašemu tenantovi služby Azure AD. To znamená, že přidání aplikace Azure AD (instančního objektu) v partnerském centru.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ef5373fd9a606cd25345cbe80a55f28fc1f753f
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028464"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Přidání aplikace Azure AD (instančního objektu) v partnerském centru

**Příslušné role**

- Globální správce

V programu komerčního obchodu v partnerském centru teď můžete do svého účtu partnerského centra přidat aplikaci Azure AD (instanční objekt) jako uživatele. (Dříve jste to mohli udělat v portál partnerů cloudu, nebo CPP. Teď, když jste migrovali do partnerského centra, je účet CPP jen pro čtení.)
 
>[!Note] 
>Instanční objekt je synonymem pro aplikaci Azure AD.

## <a name="add-an-azure-ad-application-service-principal"></a>Přidat aplikaci Azure AD (instanční objekt)

1. Z řídicího panelu partnerského centra vyberte **Nastavení** a potom vyberte **Nastavení vývojáře**.

2. Vyberte **Uživatelé** a pak vyberte **Přidat aplikace Azure AD**.

3. Vyberte existující aplikaci Azure AD nebo vytvořte novou.

4. Pokud vytvoříte novou aplikaci Azure AD, zahrňte tyto informace:  

   - **Adresa URL odpovědi**: adresa URL, kde se uživatelé můžou přihlásit k používání vaší aplikace Azure AD.

   - **Identifikátor URI ID aplikace**: logický identifikátor pro aplikaci Azure AD, který se zobrazí, když pošle žádost o jednotné přihlašování do Azure AD.

   - **Role zabezpečení**: **správce** rolí (stejné jako role Owner v CPP) a **Developer** (stejné jako role Přispěvatel v CPP) platí pro program komerčního tržiště v partnerském centru a je možné ho přidružit k této aplikaci Azure AD.  

## <a name="next-steps"></a>Další kroky

- [Přehled komerčního tržiště v partnerském centru](csp-commercial-marketplace-overview.md)