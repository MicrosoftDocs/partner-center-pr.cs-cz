---
title: Nákup softwaru a řešení od Azure Marketplace
description: Seznamte se s nástroji, které zjednodušují a zjednodušují nákupy a správu softwaru v Azure Marketplace.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 04/15/2021
ms.openlocfilehash: cfe37f26ad685ca723336d8559d15d4a64048f4b
ms.sourcegitcommit: 2ad9e61fa5b9941f927ebf44c459b6c1bd055b9d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/08/2021
ms.locfileid: "109630079"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace nákupů

Azure Marketplace mnoho nástrojů a funkcí, které zjednodušují a zjednodušují proces nákupu, fakturace a správy zásad nákupu.

## <a name="simplified-procurement"></a>Zjednodušené pořizování

Azure Marketplace zjednodušuje proces nákupu prostřednictvím různých možností. Pokud zakoupíte produkty pomocí platební karty přidružené k vašemu účtu Azure, všechny nákupy se konsoliduje na jedné faktuře a fakturuje se na vybranou platební kartu. Pokud jste velký zákazník, můžete k nákupu použít smlouva Enterprise. U smlouvy EA se všechny nákupy softwaru automaticky zahrnou na vaši fakturu za Azure. Vaše faktura bude na prvním místě obsahovat poplatky za využití Azure a následně poplatky z Azure Marketplace.

Při nákupu prostřednictvím Azure Marketplace eliminujete složitost správy vztahů a faktur jednotlivých dodavatelů. Od Microsoftu získáte jednu konsolidovanou měsíční fakturu, která zahrnuje vaše nákupy Azure Marketplace i poplatky za Azure.

## <a name="permission-to-purchase"></a>Oprávnění k nákupu

Jakmile najdete správnou softwarovou aplikaci, je dokončení nákupu jednoduché. Budete ale potřebovat vhodná oprávnění v rámci předplatného Azure. Vzhledem k tomu, že Azure [funguje na základě Access Control](/azure/role-based-access-control/overview) (RBAC),  váš účet k nákupu potřebuje oprávnění vlastníka nebo přispěvatele předplatného. 

Před dokončením nákupu se ujistěte, že má uživatel v tenantovi Azure správnou konfiguraci. To vám pomůže zabránit chybám při nákupu.

V Azure Marketplace prostředí v Azure Portal najděte aplikaci, kterou chcete koupit, a vyberte **Vytvořit** nebo **Nastavit a přihlásit k odběru.** Než budete moct nové řešení použít, zobrazí se výzva k dokončení některých informací.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Tlačítko Vytvořit nabídky.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Tlačítko Nastavit a přihlásit k odběru":::

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

## <a name="purchase-validation-checks"></a>Kontrola ověření nákupu

Nákup nabídky prostřednictvím Azure Marketplace může selhat z různých důvodů. Použití rozhraní příkazového řádku (CLI) pro nákup je pravděpodobnější, že může dojít k chybám, protože se pokoušíte koupit nabídku, která není k dispozici nebo je zobrazená v Azure Marketplace. Níže jsou uvedená kontrola, která může způsobit selhání nákupu:

1. Předplatné patří do skupiny smlouva Enterprise (EA) a správce EA zakázal Azure Marketplace nákupy.
1. Správce EA povolil nákupy jenom pro bezplatné nabídky a nabídka je placená.
1. Nabídka se na marketplace nenachová.
1. Nezávislý výrobce softwaru (ISV) nabídku přestal (dříve přestal prodávat) alespoň ve vaší oblasti.
1. Předplatné, které používáte, patří do fakturačního účtu v oblasti, ve které není nabídka dostupná.
1. Předplatné nebo fakturační účet není přidružený k platnému platebnímu nástroji (například platné platební kartě).
1. Předplatné patří k Cloud Solution Provider (CSP) a isv odmítne prodávat prostřednictvím poskytovatele CSP.
1. Privátní marketplace je pro předplatné povolené a nabídka není v seznamu povolených nabídek.
1. Nabídka je pro konkrétní zákazníky privátní nebo preview a předplatné není v seznamu povolených zákazníků.

## <a name="next-steps"></a>Další kroky

- [Vyúčtování a fakturace](billing-invoicing.md)