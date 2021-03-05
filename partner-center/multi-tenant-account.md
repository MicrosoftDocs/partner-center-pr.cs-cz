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
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124801"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Přidání a správa několika tenantů v účtu partnerského centra


**Příslušné role**

- Globální správce
- Správce účtu

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

1. Na příkazovém řádku se přihlaste jako globální správce do tenanta, kterého chcete přidružit, a pak vyberte **Potvrdit**. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Snímek obrazovky s tlačítkem potvrdit v podokně potvrdit nové přidružení Azure AD"::: 

   Po potvrzení přidružení se zobrazí zpráva **všechna sada** . Chcete-li zobrazit nově přidaného tenanta, vyberte možnost **vrátit se ke správě tenanta**. 
 
>[!NOTE]
>Nemůžete přidružit klienta k účtu, pokud je už přidružený k jinému účtu partnerského centra.


## <a name="remove-a-tenant-from-your-account"></a>Odebrání tenanta z účtu
 
1. Přihlaste se jako globální správce do [partnerského centra Microsoftu](https://partner.microsoft.com/dashboard).

1. V pravém horním rohu vyberte ikonu **Nastavení** a pak vyberte **Nastavení účtu**.

1. V levém podokně vyberte možnost **klienti**. V části **spravovat klienty Azure AD** vyberte kartu **partner** .
 
1. Vyberte **Odebrat** vedle tenanta, jehož přidružení chcete odebrat.

   :::image type="content" source="images/disassociate.png" alt-text="Snímek obrazovky aktuálních přidružení klientů a jejich odkazy pro odebrání":::

   Jak je znázorněno na předchozím snímku obrazovky, odkazy **Odebrat** jsou povolené pro všechny přidružené klienty, s výjimkou primárního tenanta a tenanta, ke kterému jste aktuálně přihlášení. 

   > [!NOTE]   
   > Když odeberete tenanta, uživatelé tohoto tenanta už nebudou mít přístup k účtu partnerského centra a odebrání můžou mít dopad na vaše kompetence. 

## <a name="next-steps"></a>Další kroky

- [Vytváření uživatelských účtů](create-user-accounts-and-set-permissions.md)






