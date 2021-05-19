---
title: Přidání tenantů k účtu partnerského centra
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se přidávat, konsolidovat nebo spravovat více tenantů Azure AD v účtu partnerského centra a zjistit, proč to budete chtít udělat.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151198"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Přidání a správa několika tenantů v účtu partnerského centra


**Příslušné role**: globální správce | Správce účtu

Tento článek popisuje, jak sloučit více tenantů Azure Active Directory (Azure AD) pro vaši společnost a pak je přidat a spravovat v účtu partnerského centra. K tomu je potřeba celá řada důvodů. Například:

- Řekněme, že vaše společnost Contoso získala jinou společnost Fabrikam. Chcete, aby tyto dvě společnosti byly oddělené, ale chcete, aby noví zaměstnanci mohli používat Partnerské centrum. V takovém případě přidružíte tenanta Azure AD nové společnosti k globálnímu účtu vašeho partnera (PGA). Toto přidružení umožňuje uživatelům v obou společnostech pracovat v partnerském centru.

- Pokud svou firmu spustíte s více než jedním klientem (například *contoso.com*, *contoso.UK* a *contoso.in*), můžete pomocí víceklientské architektury seskupovat do stejného účtu počítače.

- Pokud pokyny pro fúze a získání vyžadují, abyste mohli pracovat s klienty obou společností, použijte klienty *constoso.com* i *fabrikam.com* .

- Uživatelé kteréhokoli klienta musí být schopni:
    * Přístup k partnerskému centru pro školení, digitální stahování nebo přidružení Microsoft Certified Professional (MCP)
    * Přiřadí se role partnerského centra, jako je například správce programu Microsoft Partner Network (MPN) nebo správce pobídek.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Přidání tenanta Azure AD ke svému účtu

1. Přihlaste se jako globální správce do [partnerského centra Microsoftu](https://partner.microsoft.com/dashboard).

1. V pravém horním rohu vyberte **Nastavení**, vyberte **Nastavení účtu** a pak vyberte **klienti**.
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Snímek obrazovky s tlačítkem přidružit v podokně profilu Azure AD"::: 

1. Vyberte **přidružit** a pak určete tenanta, kterého chcete přidružit.

1. Na příkazovém řádku se přihlaste jako globální správce k tenantovi, kterého chcete přidružit, a pak vyberte **Potvrdit.** 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Snímek obrazovky s tlačítkem Potvrdit v podokně Potvrdit nové přidružení Azure AD"::: 

   Po potvrzení přidružení se zobrazí zpráva **All set (Vše** nastaveno). Pokud chcete zobrazit nově přidaného tenanta, vyberte **Return to tenant management (Vrátit se ke správě tenanta).** 
 
>[!NOTE]
>Tenanta nemůžete přidružit k účtu, pokud už je přidružený k jinému Partnerské centrum účtu.


## <a name="remove-a-tenant-from-your-account"></a>Odebrání tenanta z účtu
 
1. Přihlaste se jako globální správce k [Microsoft Partnerské centrum](https://partner.microsoft.com/dashboard).

1. V pravém horním rohu vyberte **ikonu Nastavení** a pak vyberte **Nastavení účtu**.

1. V levém podokně vyberte **Tenanti.** V **části Spravovat tenanty Azure AD** vyberte **kartu** Partner.
 
1. Vedle **tenanta,** jehož přidružení chcete odebrat, vyberte Odebrat.

   :::image type="content" source="images/disassociate.png" alt-text="Snímek obrazovky s aktuálními přidruženími tenantů a jejich odkazy Odebrat":::

   Jak je znázorněno na  předchozím snímku obrazovky, odkazy Odebrat jsou povolené pro všechny přidružené tenanty s výjimkou primárního tenanta a tenanta, ke které jste aktuálně přihlášení. 

   > [!NOTE]   
   > Když odeberete tenanta, uživatelé v tomto tenantovi už nebudou mít přístup k účtu Partnerské centrum a odebrání může mít vliv na vaše kompetence. 

## <a name="next-steps"></a>Další kroky

- [Vytváření uživatelských účtů](create-user-accounts-and-set-permissions.md)






