---
title: Jak daňové zásady ovlivňují výběr pro Azure Marketplace
description: Přečtěte si, jak daňové zásady ovlivňují výběr pro Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 19acb085b601212f1bf94316aab2b72c54aecc1a
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712949"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Jak daňové zásady ovlivňují výběr pro Azure Marketplace

**Příslušné role**
-    Globální správce
-    Správce uživatelů
-    Agent správce

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

**Scénář B** – transakce, které probíhají mezi vydavatelem založeným na USA (jak je definoval informace o daňovém profilu partnera), zákazníkovi v daňové zemi spravované společností Microsoft, kde země ukládá daň na poplatek za tržišti (zdanitelná služba). V tomto scénáři se daň za poplatek za službu Store odečte od výběr vydavatele.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Zobrazuje pracovní postup pro scénář vydaných procesů B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Vydavatel se chová jako daňová země spravovaná vydavatelem

**Scénář C** – transakce prováděné mezi vydavatelem a zákazníkem v daňové zemi spravované vydavatelem, která neukládá srážkovou daň na zákazníky. Zákazníci platí bez daně v místě prodeje a jedná se o závazek vydavatele uhradit všechny použitelné daně.

Další informace o cenách specifických pro země (například pro vyrovnání nadcházejících daní) najdete v tématu [plány a ceny pro komerční nabídky na webu Marketplace](/azure/marketplace/plans-pricing#custom-prices).

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Zobrazuje pracovní postup pro scénář vydaných procesů C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Cizí Vydavatel překládá se zákazníkem v USA.

**Scénář D** – všichni cizí vydavatelé (jak je definovala informace o daňovém profilu partnerského centra) v zemích bez smlouvy US (viz [scénář E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) prodej k zákazníkovi na bázi USA (jak je definováno adresou zákaznického účtu). Státní správa USA vyžaduje, aby se za vydavatele jménem Microsoftu srážková daň. Daň sražená z výběrů do vydavatele se vypočítá na základě ceny nabídky.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Zobrazuje pracovní postup pro scénář vypsání procesu D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Cizí Vydavatel se smlouvou přepracuje se zákazníkem v USA.

**Scénář E** – všichni zahraniční vydavatelé (jak je definovala informace o daňovém profilu partnerského centra) v zemích se SMLOUVou US, která provádí prodej na zákazníky na bázi USA (jak je definováno adresou zákaznického účtu). Státní správa USA nepožaduje od Microsoftu srážku daně jménem vydavatele.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Zobrazuje pracovní postup pro scénář vypsání procesu E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Cizí Vydavatel prodává zákazníka, který je registrovaný v EU, v zemi spravované společností Microsoft (mimo Irsko).

**Scénář F** – všechny transakce mezi cizími vydavateli a zákazníky v EU registrovaných DPH (mimo Irsko) ve Microsoft-Managed zemi. Zákazník neplatí daň na prodej.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Zobrazuje pracovní postup pro scénář pro výběr procesu F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Cizí Vydavatel prodává zákazníka, který je registrovaný v EU, v zemi spravované společností Microsoft (v Irsku).

**Scénář G** – všechny transakce mezi cizími vydavateli a zákazníky v EU registrovaných DPH (v Irsku) ve Microsoft-Managed zemi. Zákazník zaplatí irskou DPH a společnost Microsoft tuto daň vyplatí pro vládu irské vlády.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Zobrazuje pracovní postup pro scénář vydaných procesů G.":::

## <a name="next-steps"></a>Další kroky

- [Nejčastější dotazy k vydavateli](/azure/marketplace/marketplace-faq-publisher-guide)
- [Pokyny k vytvoření platebních a daňových profilů](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)