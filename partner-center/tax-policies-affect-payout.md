---
title: Jak daňové zásady ovlivňují výběr pro Azure Marketplace
description: Přečtěte si, jak daňové zásady ovlivňují výběr pro Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: a93e94912f840e4cb69c3cc834f03af1b34f19aa
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856011"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Jak daňové zásady ovlivňují výběr pro Azure Marketplace

**Příslušné role**: globální správce | Správce správy uživatelů | Agent správce

## <a name="introduction"></a>Úvod

Obchod Microsoft Commercial Marketplace má globální dosah. K transakcím dochází napříč ohraničením a v závislosti na tom, kde se nachází ISV a zákazník, se může lišit finanční důsledky. Microsoft AppSource a Azure Marketplace k určení země ISV použijte informace o daňovém profilu partnerského centra. K určení země zákazníka buď použijte fakturační údaje zákazníka, nebo pokud je zákazník v EU, používáme dvě různé informace.

Chcete-li lépe porozumět následujícím scénářům, přečtěte si tabulku s [daňovými podrobnostmi](tax-details-marketplace.md) , která ukazuje, zda společnost Microsoft shromažďuje a vyplatí daně jménem vydavatele nebo pokud tato odpovědnost patří vydavateli.

> [!NOTE]
> Všechny příklady hodnot prodejů a sazeb daně v tomto tématu jsou pouze pro ilustrativní účely, nikoli pro přesné hodnoty.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Vydavatel funguje v daňové zemi spravované společností Microsoft

**Scénář a** – transakce, které probíhají mezi vydavatelem a zákazníkem v rámci [daňové země spravované společností Microsoft](tax-details-marketplace.md#microsoft-managed-countries). Tyto transakce budou mít k dispozici přidanou daň v době prodeje a společnost Microsoft odešle tuto daň do příslušné země. Z výpočtů a výběrů nejsou zadrženy žádné daně, protože jsou daně výhradně.

Podívejte se na [scénář D](#foreign-publisher-transacts-with-us-customer) pro transakce mezi vydavatelem, který není US, a zákazníkem v USA.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Zobrazuje pracovní postup pro scénář vydaných procesů A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Publisher působí v případě daňové země spravované společností Microsoft, kde poplatek za Marketplace je služba zdanitelná.

**Scénář B** – transakce, které probíhají mezi vydavatelem založeným na USA (jak je definoval informace o daňovém profilu partnera), zákazníkovi v daňové zemi spravované společností Microsoft, kde země ukládá daň na poplatek za tržišti (zdanitelná služba). V tomto scénáři se od výplaty vydavatele odečte daň z poplatku za obchod.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Zobrazuje pracovní postup pro scénář procesu výplaty B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Transakce vydavatele v daňové zemi spravované vydavatelem

**Scénář C** – transakce, ke které došlo mezi vydavatelem a zákazníkem v zemi daně spravované vydavatelem, která zákazníkům neukládá srážkovou daň. Zákazníci neplatí v okamžiku prodeje žádnou daň a vydavatel má povinnost platit všechny příslušné daně.

Další informace o cenách pro konkrétní zemi (například pro vyrovnání nadcházejících daní) najdete v tématu Plány a [ceny pro nabídky komerčního marketplace.](/azure/marketplace/plans-pricing#custom-prices)

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Zobrazuje pracovní postup pro scénář procesu výplaty C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Transakce cizích vydavatelů u zákazníka v USA

**Scénář D** – všichni cizí vydavatelé (definovaní jejich informacemi o daňovém profilu Partnerské centrum) v zemích, které nejsou v USA (viz Scénář [E)](#foreign-publisher-with-a-treaty-transacts-with-us-customer)a prodá se zákazníkovi v USA (jak je definováno adresou jejich zákaznického účtu). Státní správa USA vyžaduje, aby za vydavatele byla srážková daň od Microsoftu. Srážka daně z výplaty vydavateli se počítá na základě ceny nabídky.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Zobrazuje pracovní postup pro scénář procesu výplaty D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Cizí vydavatel se zákazníkem v USA

**Scénář E** – všichni cizí vydavatelé (definovaní jejich informacemi o daňovém profilu Partnerské centrum) v zemích, kde zákazník v USA obchoduje se zákazníkem v USA (jak je definováno adresou jejich zákaznického účtu). Státní správa USA nevyžaduje, aby Microsoft srážkovou daň za vydavatele zatápí.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Zobrazuje pracovní postup pro scénář procesu výplaty E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Cizí vydavatel prodává zákazníkovi zaregistrovanému k DPH v zemi spravované Microsoftem (mimo Irsko).

**Scénář F** – všechny transakce mezi cizími vydavateli a zákazníky registrovanými k DPH v EU (mimo Irsko) v Microsoft-Managed zemi. Zákazník při prodeji neplatí daň.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Zobrazuje pracovní postup pro scénář procesu výplaty F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Cizí Vydavatel prodává zákazníka, který je registrovaný v EU, v zemi spravované společností Microsoft (v Irsku).

**Scénář G** – všechny transakce mezi cizími vydavateli a zákazníky v EU registrovaných DPH (v Irsku) ve Microsoft-Managed zemi. Zákazník zaplatí irskou DPH a společnost Microsoft tuto daň vyplatí pro vládu irské vlády.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Zobrazuje pracovní postup pro scénář vydaných procesů G.":::

## <a name="next-steps"></a>Další kroky

- [Nejčastější dotazy k vydavateli](/azure/marketplace/marketplace-faq-publisher-guide)
- [Pokyny k vytvoření platebních a daňových profilů](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)