---
title: Jak postupovat, pokud jediný správce programu MPN opustil společnost?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak najít nového správce MPN nebo získat pomoc od globálního správce vaší společnosti. Přečtěte si také, jak přidat nového globálního správce centra partnerů.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5efd157078acd72ca47418aaa9559a678fc5b129
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151164"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>Jak postupovat, pokud jediný správce programu MPN opustil společnost?

**Příslušné role**: správce partnerů MPN | Správce účtu | Globální správce

Následující článek vás provede třemi typickými scénáři týkajícími se toho, co dělat, když váš správce programu MPN opustil společnost.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Scénář 1: správce partnerského serveru MPN nebo správce účtu společnosti, ale v účtu stále existují globální správci.

V takovém případě může být jiná osoba ve společnosti přiřazena role správce partnerů MPN. Má být přiřazená role konkrétní role správce účtu MPN partner/správce účtu:

1. Přihlaste se k účtu partnerského centra pomocí pracovního účtu (například tom@contoso.com ).
1. Z filtru stránky **správy uživatelů** u globálního správce Zjistěte, kdo jsou globální správci vaší společnosti. 
1. Obraťte se na jednoho z globálních správců a požádejte ho, aby vám přiřadil určitou roli MPN, kterou potřebujete. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Scénář 2: správce účtu MPN partner/správce účtů opustil společnost a v účtu neexistují žádní globální správci. 

Pokud přejdete na stránku **správy uživatelů** a filtr pro globální správu, ale zjistíte, že ve vaší společnosti není žádný globální správce, který vám může pomáhat získat roli určenou pro MPN, postupujte takto:

1. Přejít na [Portal.Azure.com](https://ms.portal.azure.com/), přihlaste se pomocí svého pracovního účtu (například tom@contoso.com ). 
1. V nabídce vlevo v levém navigačním panelu vyberte možnost **help + Support (podpora** ).
1. Na další stránce vyberte v rozevírací nabídce **nový typ support Request** a typ **technického problému** , vložte další podrobnosti a klikněte na **Další: řešení.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Vyhledat správce v Azure Portal":::

4. Po kontrole doporučených řešení na další stránce vyberte **Další: podrobnosti** a vyplňte potřebná pole.
1. Zkontrolujte a vytvořte žádost o podporu.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Scénář 3: správce partnerského serveru MPN/správce účtu nebo globální správce opustil společnost a neexistují žádní jiní uživatelé, kteří mají přístup k Azure AD společnosti. To je úplná ztráta přístupu.

Postupujte podle kroků [převzetí správce](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) , které převezmou nespravovaný adresář jako správce Azure Active Directory.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Nejste si jistí, jestli má vaše společnost již pracovní účet?

Pokud si nejste jistí, jestli má vaše společnost pracovní účet, proveďte kontrolu pomocí těchto kroků.

1. Přihlaste se k [portálu pro správu Azure](https://ms.portal.azure.com).
2. V nabídce vlevo vyberte **Azure Active Directory** a pak vyberte **názvy domén**.
Pokud již máte pracovní účet, bude uveden název vaší domény.

>[!Note]
>Pokud máte aktivní předplatné Microsoft Azure nebo Office 365, již máte pracovní účet a přihlašovací údaje pro přihlášení by měly být stejné jako ty, které se používají pro přístup k těmto službám.