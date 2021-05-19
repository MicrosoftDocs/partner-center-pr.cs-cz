---
title: Vytváření uživatelských účtů a přiřazování rolí
description: Každý zaměstnanec musí mít přiřazenou roli, aby mohl získat přístup k partnerskému centru. Naučte se vytvářet uživatelské účty, přiřazovat role a nastavovat oprávnění.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 9621f0bc3283d7d3b08e2ebac62b4e5d8c95a4d4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148138"
---
# <a name="create-user-accounts"></a>Vytváření uživatelských účtů  

**Příslušné role**: správce účtu | Globální správce | Správce správy uživatelů

Vytvořte uživatelské účty pro zaměstnance, kteří potřebují přístup k partnerskému centru. Tyto úlohy musí provádět správce správy uživatelů, účty správce nebo globální správce. Uživatel, který provádí tyto úlohy, musí také přiřadit role Azure Active Directory (AAD) Správce uživatelů nebo globální správce. Další informace o rolích AAD najdete v tématu [oprávnění role správce v Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).

## <a name="add-a-new-user"></a>Přidání nového uživatele

1. Z ikony **Nastavení** v pravém horním rohu partnerského centra vyberte **Nastavení účtu** a pak vyberte **Správa uživatelů**.

2. Vyberte možnost **Přidat uživatele**.

3. Zadejte celé jméno uživatele a jedinečnou e-mailovou adresu.

4. Vyberte typ agenta nebo typu správce, kterého chcete přiřadit uživateli. Přístup k partnerskému centru je založený na rolích, takže můžete přiřadit oprávnění k přizpůsobení zobrazení uživatele, aby se zobrazily jenom ty funkce, které uživatel potřebuje k dokončení konkrétních úkolů.  Pokud uživatelé chtějí přiřazení role, můžou najít globální správce, aby se obrátili na **správu uživatelů** a filtrování na globálním správci.

5. Výběrem **Přidat** vytvořte uživatelský účet. Potvrďte podrobnosti uživatele na další stránce.

> [!IMPORTANT]  
> Poznamenejte si informace o přihlášení nového uživatele zobrazené na této stránce. Nezapomeňte tyto informace zkopírovat a odeslat novému uživateli, protože k němu už nebudete mít přístup později. 

Uživatel se bude muset přihlásit do partnerského centra s uživatelským jménem a dočasným heslem. Když se uživatel poprvé přihlásí k partnerskému centru, zobrazí se výzva ke změně hesla.

## <a name="assign-user-roles"></a>Přiřazení uživatelských rolí

Pokud chcete pracovat v partnerském centru, musíte mít přiřazenou roli.  V současné době role zahrnují Azure Active Directory role tenanta, role poskytovatele Cloud Solution Provider (CSP) a role společnosti bez AAD. Všechny tyto role může potřebovat jednotlivá společnost.

>[!Important]
>Jednotlivci musí být uvedeni ve vašem tenantovi, aby k Partnerské centrum. Přiřazení rolí poskytují další přístup.

## <a name="next-steps"></a>Další kroky

- [Přiřazení rolí a oprávnění uživatelů pro zaměstnance, kteří potřebují pracovat v Partnerské centrum](permissions-overview.md)
