---
title: Nákup softwaru a řešení od Azure Marketplace
description: Seznamte se s nástroji, které zjednodušují a zjednodušují nákupy a správu softwaru v Azure Marketplace.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: 11145280aad1ecd9777ec2fb7540e7d6479acfae
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431545"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace nákupů

Azure Marketplace mnoho nástrojů a funkcí, které zjednodušují a zjednodušují proces nákupu, fakturace a správy zásad nákupu.

## <a name="simplified-procurement"></a>Zjednodušené pořizování

Azure Marketplace zjednodušuje proces nákupu prostřednictvím různých možností. Pokud zakoupíte produkty pomocí platební karty přidružené k vašemu účtu Azure, všechny nákupy se konsoliduje na jedné faktuře a fakturuje se na vybranou platební kartu. Pokud jste velký zákazník, můžete k nákupu použít smlouva Enterprise. U smlouvy EA se všechny nákupy softwaru automaticky zahrnou na vaši fakturu za Azure. Vaše faktura bude na prvním místě obsahovat poplatky za využití Azure a následně poplatky z Azure Marketplace.

Při nákupu prostřednictvím Azure Marketplace eliminujete složitost správy vztahů a faktur jednotlivých dodavatelů. Získáte jednu konsolidovanou měsíční fakturu od Microsoftu, která zahrnuje jak vaše nákupy Azure Marketplace, tak poplatky za Azure.

## <a name="permission-to-purchase"></a>Oprávnění k nákupu

Jakmile najdete správnou softwarovou aplikaci, je dokončení nákupu jednoduché. Budete ale potřebovat vhodná oprávnění v rámci předplatného Azure. Vzhledem k tomu, že Azure [funguje na základě Access Control](/azure/role-based-access-control/overview) (RBAC),  váš účet k nákupu potřebuje oprávnění vlastníka nebo přispěvatele předplatného. 

Před dokončením nákupu se ujistěte, že má uživatel v tenantovi Azure správnou konfiguraci. To vám pomůže zabránit chybám při nákupu.

V Azure Marketplace prostředí v Azure Portal najděte aplikaci, kterou chcete koupit, a vyberte **Vytvořit** nebo **Nastavit a přihlásit k odběru.** Než budete moct nové řešení použít, zobrazí se výzva k dokončení některých informací.

> [!CAUTION]
> Schválení na privátním marketplace neznačí nákup řešení.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Tlačítko Vytvořit nabídky.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Tlačítko Nastavit a přihlásit k odběru":::

Pokud chcete nasadit řešení z online obchodu Azure Marketplace,  na stránce s popisem produktu vyberte Získat a pak se přihlaste pomocí svých přihlašovacích údajů k účtu Azure.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Dialogové Azure Marketplace přihlášení.":::

Po přihlášení budete přesměrováni na produkt v Azure Portal dokončíte nákup.

## <a name="purchase-policy-management"></a>Správa zásad nákupu

Microsoft umožňuje spravovat nákupy uživatelů prostřednictvím fakturačního profilu jako správce předplatného Azure. Vyberte si ze tří možností:

- **Free + Paid** – umožňuje uživatelům získat jakoukoli Azure Marketplace aplikace.
- **Free** – umožňuje uživatelům nasazovat jenom bezplatný software z Azure Marketplace.
- **Ne** – Zabrání uživatelům v nasazení jakéhokoli softwaru z Azure Marketplace.

Tato nastavení platí pro všechny uživatele s přístupem k vašemu předplatnému Azure, což vám dává možnost řídit nákup IT prostřednictvím Azure Portal.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Řízení nákupů IT prostřednictvím Azure Portal.":::

## <a name="cost-management"></a>Správa nákladů

Při nákupu produktů z Azure Marketplace chcete získat přehledy, které vám pomůžou spravovat náklady. Azure Cost Management je bezplatný nástroj pro zobrazení informací o zakoupených produktech. Pomocí této Cost Management můžete zobrazit podrobnosti o tom, za jaké služby v průběhu času utrácíte peníze a jak tyto náklady sledují oproti rozpočtům, které jste nastavili. Kromě nastavení rozpočtů můžete plánovat sestavy a analyzovat náklady na předplatné. Další informace o Azure Cost Management najdete v modulu Microsoft Learn o analýze nákladů a vytváření rozpočtů [pomocí Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

V nástroji pro analýzu nákladů v rámci služby Azure Cost Management si můžete zobrazit poplatky a faktury z Azure Marketplace.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Pomocí Azure Cost Management můžete získat přehled o zakoupených produktech.":::

## <a name="purchase-validation-checks"></a>Kontrola ověření nákupu

Nákup nabídky prostřednictvím Azure Marketplace může selhat z různých důvodů. Použití rozhraní příkazového řádku (CLI) k nákupu s větší pravděpodobností způsobí chyby, protože se možná pokoušíte koupit nabídku, která není dostupná nebo viditelná v Azure Marketplace. Níže jsou uvedená kontrola, která může způsobit selhání nákupu:

1. Předplatné patří do skupiny smlouva Enterprise (EA) a správce EA zakázal Azure Marketplace nákupy.
1. Správce EA povolil nákupy jenom pro bezplatné nabídky a nabídka je placená.
1. Nabídka se na marketplace nenachová.
1. Nezávislý výrobce softwaru (ISV) přestal nabídku prodávat, alespoň ve vaší oblasti.
1. Předplatné, které používáte, patří do fakturačního účtu v oblasti, ve které není nabídka dostupná.
1. Předplatné nebo fakturační účet není přidružený k platnému platebnímu nástroji (například platné platební kartě).
1. Předplatné patří k Cloud Solution Provider (CSP) a isv odmítne prodávat prostřednictvím poskytovatele CSP.
1. Privátní marketplace je pro předplatné povolené a nabídka není v seznamu povolených nabídek.
1. Nabídka je pro konkrétní zákazníky privátní nebo preview a předplatné není v seznamu povolených zákazníků.

## <a name="next-steps"></a>Další kroky

- [Vyúčtování a fakturace](billing-invoicing.md)