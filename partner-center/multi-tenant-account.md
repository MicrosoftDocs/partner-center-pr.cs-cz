---
title: Přidání dalších tenantů k účtu partnerského centra
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se přidávat, konsolidovat a spravovat více tenantů Azure AD v účtu partnerského centra. Seznamte se také s některými důvody, které byste mohli chtít udělat.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/19/2020
ms.locfileid: "92527751"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Přidání a správa několika tenantů v účtu partnerského centra

**Platí pro**

- Partnerské centrum

**Příslušné role**

- Globální správce

Tato funkce umožňuje spravovat více tenantů vaší společnosti a konsolidovat je do vašeho účtu v Partnerském centru. Existuje mnoho důvodů, proč možná budete muset ve svém účtu partnerského centra spravovat více tenantů Azure AD. Příklad:

- Vaše společnost si může koupit jinou společnost a vy chcete, aby zaměstnanci v nové firmě mohli používat Partnerské centrum. Chcete však, aby tyto dvě společnosti byly oddělené. V takovém případě přiřadíte tenanta Azure AD nové společnosti k vašemu globálnímu účtu vašeho partnera (PGA). Toto přidružení umožní uživatelům v obou společnostech pracovat v partnerském centru.

- Pokud máte více než jednoho tenanta pro provozování vaší firmy (např. contoso.com, contoso.uk, contoso.in), můžete použít víceklientské prostředí, abyste je mohli spojit se stejným účtem počítače.

- Fúze a akvizice vyžaduje, abyste pracovali s více než jedním klientem (např. Pokud společnost Contoso získá společnost Fabrikam, budete muset použít jak Constoso.com, tak Fabrikam.com příslušného tenanta).

- Uživatelé ze všech tenantů by museli mít tyto možnosti:
    1.  Přístup k partnerským centrům pro školení, digitální stahování, MCP přidružení
    2.  Přiřadí se role partnerského centra, jako je například správce programu MPN, pobídka správce atd.


## <a name="add-another-azure-ad-tenant-to-your-account"></a>Přidat do svého účtu jiného tenanta Azure AD

1. Jako globální správce se přihlaste do [řídicího panelu](https://partner.microsoft.com/dashboard)partnerského centra.
1. V ikoně **Nastavení** vyberte **Nastavení účtu** a pak vyberte **klienti** .
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="přidružit klienty"::: 

3. Vyberte **přidružit jiného tenanta služby AD** a určete tenanta, kterého chcete přidružit.

1. Jako globální správce se přihlaste ke klientovi, kterého chcete přidružit, a potvrďte přidružení. 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="přidružit klienty"::: 

5. Po potvrzení se zobrazí všechna oznámení o **sadě** .  Vyberte možnost **vrátit se ke správě tenanta** a zobrazí se nově přidaný tenant. 
 

>[!NOTE]
>Tenanta nemůžete přidružit k účtu, pokud je už přidružený k jinému účtu partnerského centra.

 
## <a name="next-steps"></a>Další kroky

- [Přidávání uživatelů](create-user-accounts-and-set-permissions.md)
