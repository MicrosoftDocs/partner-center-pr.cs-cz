---
title: Vliv daňových zásad na výplatu Azure Marketplace
description: Přečtěte si, jak daňové zásady ovlivňují výplatu Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 343db43633245030a5eba213cb5c8b79d09a7dee
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686309"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Vliv daňových zásad na výplatu Azure Marketplace

**Odpovídající role**

- Globální správce
- Správce správy uživatelů
- Agent pro správu

## <a name="introduction"></a>Úvod

Komerční marketplace Microsoftu má globální dosah. Transakce prochádnou přes hranice a v závislosti na tom, kde se nachází isv a zákazník, se můžou daňové důsledky lišit. Microsoft AppSource a Azure Marketplace země isV Partnerské centrum informace o daňovém profilu. K určení země zákazníka použijte buď fakturační údaje zákazníka, nebo , pokud je zákazník v EU, používáme dva různé údaje.

Pokud chcete lépe porozumět následujícím [](tax-details-marketplace.md) scénářům, přečtěte si tabulku Podrobnosti o daních, která ukazuje, jestli Microsoft shromažďuje a platí daně jménem vydavatele nebo jestli tato odpovědnost patří vydavateli.

> [!NOTE]
> Všechny příklady hodnot prodeje a procentuální hodnoty daně v tomto tématu jsou pouze pro ilustrativní účely, nikoli pro přesné hodnoty.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Transakce vydavatelů v daňové zemi spravované Microsoftem

**Scénář A** – transakce, ke které došlo mezi vydavatelem a zákazníkem v daňové zemi [spravované Microsoftem](tax-details-marketplace.md#microsoft-managed-countries) U těchto transakcí se při prodeji přidá příslušná daň a Microsoft ji odešle příslušné zemi. Nezachytají se žádné daně z výplaty a výpočty výplat se vylučují z daní.

Informace [o transakcích mezi](#foreign-publisher-transacts-with-us-customer) vydavatelem mimo USA a zákazníkem v USA najdete v tématu Scénář D.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Zobrazuje pracovní postup pro scénář procesu výplaty A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Transakce vydavatele v daňové zemi spravované Microsoftem, kde poplatky za Marketplace jsou daňové služby

**Scénář B** – transakce, které procháznou mezi vydavatelem v USA (podle definice v informacích o jejich daňovém profilu Partnerské centrum) se zákazníkovi v daňové zemi spravované Microsoftem, ve které země ukládá daň na poplatek za Marketplace (službu, která se má daň). V tomto scénáři se daň za poplatek za službu Store odečte od výběr vydavatele.

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

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Cizí vydavatel prodává zákazníkovi zaregistrovanému k DPH v zemi spravované Microsoftem (v Zemích).

**Scénář G** – všechny transakce mezi cizími vydavateli a zákazníky registrovanými k DPH v EU (uvnitř Microsoft-Managed země). Zákazník platí DPH a Microsoft tuto daň vyplácí státní správy.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Zobrazuje pracovní postup pro scénář procesu výplaty G.":::

## <a name="next-steps"></a>Další kroky

- [Nejčastější dotazy k vydavateli](/azure/marketplace/marketplace-faq-publisher-guide)
- [Pokyny k vytvoření platebního a daňového profilu](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)