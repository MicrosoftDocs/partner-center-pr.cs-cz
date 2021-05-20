---
title: Vyhledání ID tenanta, názvu domény, ID objektu uživatele
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak najít ID v Azure Portal – ID tenanta Azure AD organizace, název domény nebo ID konkrétního objektu uživatele. Některé úlohy tyto informace potřebují.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150858"
---
# <a name="locate-important-ids-for-a-user"></a>Vyhledání důležitých ID pro uživatele

**Odpovídající role:** Globální správce

Tento článek popisuje, jak pomocí [Azure Portal](https://portal.azure.com/) najít pro uživatele následující informace:

- ID Microsoft Azure Active Directory (Azure AD) organizace nebo společnosti uživatele

- Primární název domény organizace nebo společnosti přidružené k tenantovi Azure AD

- ID objektu uživatele

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Vyhledání ID Microsoft Azure AD tenanta a názvu primární domény

Pomocí následujícího postupu vyhledejte ID tenanta Azure AD nebo název primární domény v rámci Azure Portal. (Pokud chcete ID tenanta najít programově, podívejte se na stránku Vyhledání ID tenanta pomocí [PowerShellu nebo rozhraní příkazového řádku](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)

> [!NOTE]
> ID tenanta se v různých aplikacích nebo zdrojích může nazývat různé názvy. ID tenanta může být například označováno jako ID adresáře, tenant Azure Active Directory (Azure AD), MICROSOFT ID nebo pro určité sestavy, a to i *tenantguid*.

1. Přihlaste se na [Azure Portal](https://portal.azure.com/).

2. V **Azure Active Directory** vyberte Další.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Zobrazuje Azure Portal výběrem Azure Active Directory v nabídce.":::

3. Zobrazí Azure Active Directory **přehledu.** Pokud chcete najít ID tenanta Azure AD nebo název primární domény, vyhledejte pole **ID tenanta** a **pole Primární** doména. Tato pole se zobrazí v části Informace o tenantovi.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Zobrazuje stránku Přehled se dvěma zvýrazněných poli: ID tenanta a název primární domény.":::

4. ID tenanta můžete najít v Azure Portal několika dalšími způsoby. V nabídce vyberte **Azure Active Directory** . Pak v nabídce Najděte oddíl **Spravovat** a vyberte **vlastnosti**.

   Na stránce vlastnosti se zobrazí také přidružené ID tenanta uživatele.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Zobrazí stránku vlastností se zvýrazněným polem ID tenanta.":::

## <a name="find-the-user-object-id"></a>Najít ID objektu uživatele

Stačí najít název domény a ID tenanta nemusí být vždy dostatek. Může být také nutné vyhledat konkrétní ID objektu přiřazené uživateli. Pomocí těchto kroků můžete najít ID objektu uživatele v Azure Portal:

1. Přihlaste se na [Azure Portal](https://portal.azure.com/).

2. V nabídce vyberte **Azure Active Directory** .

3. V nabídce najděte část **Správa** a pak vyberte **Uživatelé**.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Zobrazí nabídku Azure Active Directory se zvýrazněnou možností uživatelé.":::

4. Na stránce Uživatelé zadejte do vyhledávacího pole jméno uživatele.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Zobrazí stránku Uživatelé s vyhledávacím polem pro vyhledání konkrétního uživatele.":::

5. Vyberte jméno uživatele, kde se zobrazí v seznamu.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Zobrazí stránku uživatele zobrazující řádek vyhledávaného uživatele.":::

6. Na stránce profilu uživatele Najděte oddíl identita. Tady se zobrazí pole ID objektu s jedinečným ID objektu uživatele.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Zobrazuje stránku profilu uživatele s částí identita a jedno zvýrazněné pole pro ID objektu.":::

## <a name="next-steps"></a>Další kroky

- [Programové zjištění ID tenanta pomocí PowerShellu nebo rozhraní příkazového řádku](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Další informace o uživatelských profilech v Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Zjistěte, jak můžou partneři zobrazit nebo exportovat podrobnosti o zákaznících v partnerském centru.](see-your-customer-list.md)

