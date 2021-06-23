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
ms.openlocfilehash: 3698032a632384e8416664c9564819d7c4da9c38
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551550"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Přidání aplikace Azure AD (instančního objektu) v partnerském centru

**Příslušné role**: globální správce

V programu pro komerční tržiště v partnerském centru teď můžete do svého účtu partnerského centra přidat aplikaci Microsoft Azure Active Directory (Azure AD) (instanční objekt) jako uživatele. (To jste na svém účtu portál partnerů cloudu (CPP) mohli provést dříve. Teď, když jste migrovali do partnerského centra, je účet CPP jen pro čtení.)
 
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