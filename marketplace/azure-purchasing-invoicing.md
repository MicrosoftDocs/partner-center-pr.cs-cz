---
title: Nákup softwaru a řešení z Azure Marketplace
description: Seznamte se s nástroji, které zjednodušují a zjednodušují nákupy a správu softwaru v Azure Marketplace.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 8f7962b1b040be90f7dc1b2696a2ced3830d25b9
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182473"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace nákupu

Azure Marketplace má mnoho nástrojů a funkcí, které zjednodušují a zjednodušují proces nákupu, fakturace a správy zásad nákupu.

## <a name="simplified-procurement"></a>Zjednodušená zakázka

Azure Marketplace zjednodušuje proces nákupu prostřednictvím různých možností. Pokud si koupíte produkty pomocí platební karty přidružené k vašemu účtu Azure, budou se všechny nákupy konsolidovat na jednu fakturu a budou se fakturovat na základě kreditní karty, kterou si zvolíte. Pokud jste velký zákazník, můžete si ho koupit pomocí smlouva Enterprise. V případě smlouvy EA jsou veškeré nákupy softwaru automaticky zahrnuté do vaší faktury Azure. Vaše faktura bude na prvním místě obsahovat poplatky za využití Azure a následně poplatky z Azure Marketplace.

Při nákupu prostřednictvím Azure Marketplace Eliminujte složitost správy vztahů a faktur jednotlivých dodavatelů. Získáte jednu konsolidovanou měsíční fakturu od Microsoftu, která zahrnuje nákupy Azure Marketplace i poplatky za Azure.

## <a name="permission-to-purchase"></a>Oprávnění k nákupu

Po nalezení správné softwarové aplikace je dokončení nákupu jednoduché. V rámci předplatného Azure ale budete potřebovat vhodná oprávnění. Vzhledem k tomu, že Azure pracuje na modelu správy [Access Control na základě rolí](/azure/role-based-access-control/overview) (RBAC), váš účet potřebuje k nákupu nákup oprávnění vlastníka nebo **přispěvatele** **předplatného** .

Před dokončením nákupu se ujistěte, že uživatel má v tenantovi Azure správnou konfiguraci. To vám pomůže zabránit chybám při nákupu.

V prostředí Azure Marketplace v Azure Portal Najděte aplikaci, kterou chcete koupit, a vyberte **vytvořit** nebo **nastavit + předplatné**. Před tím, než budete moci použít nové řešení, budete vyzváni k dokončení některých informací.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Tlačítko pro vytvoření nabídky":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Tlačítko nastavit + odběr.":::

Pokud chcete nasadit řešení z Azure Marketplace online obchodu, vyberte **získat** na stránce Popis produktu a pak se přihlaste pomocí svých přihlašovacích údajů k účtu Azure.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Přihlašovací dialogové okno Azure Marketplace.":::

Až se přihlásíte, budete přesměrováni na produkt v Azure Portal k dokončení nákupu.

## <a name="purchase-policy-management"></a>Správa zásad nákupu

Microsoft vám umožňuje spravovat nákupy uživatelů prostřednictvím vašeho fakturačního profilu jako správce předplatného Azure. Vyberte si ze tří možností:

- **Zdarma + placená** – umožní uživatelům získat jakoukoli Azure Marketplace softwarovou aplikaci.
- **Zdarma** – umožňuje uživatelům nasadit jenom bezplatný software z Azure Marketplace.
- **Ne** – zabrání uživatelům v nasazení jakéhokoli softwaru z Azure Marketplace.

Tato nastavení platí pro všechny uživatele, kteří mají přístup k vašemu předplatnému Azure, což vám dává možnost řídit si jejich nákup prostřednictvím Azure Portal.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Řízení jejich nákupu prostřednictvím Azure Portal":::

## <a name="cost-management"></a>Správa nákladů

Při nákupu produktů od Azure Marketplace chcete získat přehledy, které vám pomůžou se správou nákladů. Azure Cost Management je bezplatný nástroj pro zobrazení informací o produktech, které jste zakoupili. Pomocí Cost Management můžete zobrazit podrobné informace o tom, jaké služby strávíte v průběhu času a jak se tyto náklady budou sledovat s rozpočty, které jste nastavili. Kromě nastavení rozpočtů můžete plánovat sestavy a analyzovat náklady na předplatné. Přečtěte si další informace o Azure Cost Management tím, že Microsoft Learn modul [vyplníte o analýzu nákladů a vytvoříte rozpočty s Azure cost management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

V nástroji pro analýzu nákladů v rámci služby Azure Cost Management si můžete zobrazit poplatky a faktury z Azure Marketplace.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Pomocí Azure Cost Management můžete získat přehled o zakoupených produktech.":::

## <a name="next-steps"></a>Další kroky

- [Vyúčtování a fakturace](billing-invoicing.md)