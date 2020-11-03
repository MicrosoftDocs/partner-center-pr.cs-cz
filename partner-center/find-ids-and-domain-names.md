---
title: Najít ID tenanta, název domény, ID objektu uživatele
ms.topic: how-to
ms.date: 09/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak najít ID v Azure Portal-ID tenanta služby Azure AD, název domény nebo konkrétní ID objektu uživatele v organizaci. Tyto informace vyžadují některé úlohy.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4a3695079a9d5b0b3c66b7c2eda52a31888a6660
ms.sourcegitcommit: 3158b0de261539694e37e433c763afa4067e36fb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/17/2020
ms.locfileid: "92527258"
---
# <a name="locate-important-ids-for-a-user"></a>Vyhledat důležitá ID pro uživatele

Tento článek popisuje, jak pomocí [Azure Portal](https://portal.azure.com/) najít pro uživatele následující informace:

- ID tenanta Microsoft Azure Active Directory (Azure AD) organizace nebo společnosti uživatele

- Primární název domény organizace nebo společnosti přidružené k tenantovi Azure AD

- ID objektu uživatele

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Najít ID tenanta Microsoft Azure AD a název primární domény

Při hledání ID tenanta Azure AD nebo názvu primární domény v rámci Azure Portal postupujte podle těchto kroků.

> [!NOTE]
> ID tenanta se může v různých aplikacích a prostředcích volat jako jiné názvy. ID klienta může být například označováno jako ID adresáře, tenant Azure Active Directory (Azure AD), Microsoft ID nebo pro určité sestavy, a to i pro *tenantguid* .

1. Přihlaste se k webu [Azure Portal](https://portal.azure.com/).

2. V nabídce vyberte **Azure Active Directory** .

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Zobrazuje Azure Portal výběru možnosti Azure Active Directory z nabídky.":::

3. Zobrazí se stránka s **přehledem** Azure Active Directory. Pokud chcete najít ID tenanta služby Azure AD nebo název primární domény, vyhledejte pole **ID tenanta** a **Primární doména** . Tato pole se zobrazí v části informace o Tenantovi.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Zobrazuje Azure Portal výběru možnosti Azure Active Directory z nabídky.":::

4. ID tenanta můžete najít v Azure Portal několika dalšími způsoby. V nabídce vyberte **Azure Active Directory** . Pak v nabídce Najděte oddíl **Spravovat** a vyberte **vlastnosti** .

   Na stránce vlastnosti se zobrazí také přidružené ID tenanta uživatele.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Zobrazuje Azure Portal výběru možnosti Azure Active Directory z nabídky.":::

## <a name="find-the-user-object-id"></a>Najít ID objektu uživatele

Stačí najít název domény a ID tenanta nemusí být vždy dostatek. Může být také nutné vyhledat konkrétní ID objektu přiřazené uživateli. Pomocí těchto kroků můžete najít ID objektu uživatele v Azure Portal:

1. Přihlaste se k webu [Azure Portal](https://portal.azure.com/).

2. V nabídce vyberte **Azure Active Directory** .

3. V nabídce najděte část **Správa** a pak vyberte **Uživatelé** .

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Zobrazuje Azure Portal výběru možnosti Azure Active Directory z nabídky.":::

4. Na stránce Uživatelé zadejte do vyhledávacího pole jméno uživatele.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Zobrazuje Azure Portal výběru možnosti Azure Active Directory z nabídky.":::

5. Vyberte jméno uživatele, kde se zobrazí v seznamu.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Zobrazuje Azure Portal výběru možnosti Azure Active Directory z nabídky.":::

6. Na stránce profilu uživatele Najděte oddíl identita. Tady se zobrazí pole ID objektu s jedinečným ID objektu uživatele.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Zobrazuje Azure Portal výběru možnosti Azure Active Directory z nabídky.":::

## <a name="next-steps"></a>Další kroky

- [Další informace o uživatelských profilech v Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Zjistěte, jak můžou partneři zobrazit nebo exportovat podrobnosti o zákaznících v partnerském centru.](see-your-customer-list.md)