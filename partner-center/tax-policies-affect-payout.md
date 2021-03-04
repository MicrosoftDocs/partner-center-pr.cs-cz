---
title: Jak daňové zásady ovlivňují výběr pro Azure Marketplace
description: Přečtěte si, jak daňové zásady ovlivňují výběr pro Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 3630824c839ccd9f54f3e8e5199a573b5824bb91
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/03/2021
ms.locfileid: "101758874"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="f06a2-103">Jak daňové zásady ovlivňují výběr pro Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f06a2-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="f06a2-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="f06a2-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="f06a2-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="f06a2-105">Global admin</span></span>
-    <span data-ttu-id="f06a2-106">Správce uživatelů</span><span class="sxs-lookup"><span data-stu-id="f06a2-106">User admin</span></span>
-    <span data-ttu-id="f06a2-107">Agent správce</span><span class="sxs-lookup"><span data-stu-id="f06a2-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="f06a2-108">Úvod</span><span class="sxs-lookup"><span data-stu-id="f06a2-108">Introduction</span></span>

<span data-ttu-id="f06a2-109">Obchod Microsoft Commercial Marketplace má globální dosah.</span><span class="sxs-lookup"><span data-stu-id="f06a2-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="f06a2-110">K transakcím dochází napříč ohraničením a v závislosti na tom, kde se nachází ISV a zákazník, se může lišit finanční důsledky.</span><span class="sxs-lookup"><span data-stu-id="f06a2-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="f06a2-111">Microsoft AppSource a Azure Marketplace k určení země ISV použijte informace o daňovém profilu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="f06a2-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="f06a2-112">K určení země zákazníka buď použijte fakturační údaje zákazníka, nebo pokud je zákazník v EU, používáme dvě různé informace.</span><span class="sxs-lookup"><span data-stu-id="f06a2-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="f06a2-113">Chcete-li lépe porozumět následujícím scénářům, přečtěte si tabulku s [daňovými podrobnostmi](tax-details-marketplace.md) , která ukazuje, zda společnost Microsoft shromažďuje a vyplatí daně jménem vydavatele nebo pokud tato odpovědnost patří vydavateli.</span><span class="sxs-lookup"><span data-stu-id="f06a2-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="f06a2-114">Všechny příklady hodnot prodejů a sazeb daně v tomto tématu jsou pouze pro ilustrativní účely, nikoli pro přesné hodnoty.</span><span class="sxs-lookup"><span data-stu-id="f06a2-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="f06a2-115">Vydavatel funguje v daňové zemi spravované společností Microsoft</span><span class="sxs-lookup"><span data-stu-id="f06a2-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="f06a2-116">**Scénář a** – transakce, které probíhají mezi vydavatelem a zákazníkem v rámci [daňové země spravované společností Microsoft](tax-details-marketplace.md#microsoft-managed-countries).</span><span class="sxs-lookup"><span data-stu-id="f06a2-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="f06a2-117">Tyto transakce budou mít k dispozici přidanou daň v době prodeje a společnost Microsoft odešle tuto daň do příslušné země.</span><span class="sxs-lookup"><span data-stu-id="f06a2-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="f06a2-118">Z výpočtů a výběrů nejsou zadrženy žádné daně, protože jsou daně výhradně.</span><span class="sxs-lookup"><span data-stu-id="f06a2-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="f06a2-119">Podívejte se na [scénář D](#foreign-publisher-transacts-with-us-customer) pro transakce mezi vydavatelem, který není US, a zákazníkem v USA.</span><span class="sxs-lookup"><span data-stu-id="f06a2-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Zobrazuje pracovní postup pro scénář vydaných procesů A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="f06a2-121">Publisher působí v případě daňové země spravované společností Microsoft, kde poplatek za Marketplace je služba zdanitelná.</span><span class="sxs-lookup"><span data-stu-id="f06a2-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="f06a2-122">**Scénář B** – transakce, které probíhají mezi vydavatelem založeným na USA (jak je definoval informace o daňovém profilu partnera), zákazníkovi v daňové zemi spravované společností Microsoft, kde země ukládá daň na poplatek za tržišti (zdanitelná služba).</span><span class="sxs-lookup"><span data-stu-id="f06a2-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="f06a2-123">V tomto scénáři se daň za poplatek za službu Store odečte od výběr vydavatele.</span><span class="sxs-lookup"><span data-stu-id="f06a2-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Zobrazuje pracovní postup pro scénář vydaných procesů B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="f06a2-125">Vydavatel se chová jako daňová země spravovaná vydavatelem</span><span class="sxs-lookup"><span data-stu-id="f06a2-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="f06a2-126">**Scénář C** – transakce prováděné mezi vydavatelem a zákazníkem v daňové zemi spravované vydavatelem, která neukládá srážkovou daň na zákazníky.</span><span class="sxs-lookup"><span data-stu-id="f06a2-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="f06a2-127">Zákazníci platí bez daně v místě prodeje a jedná se o závazek vydavatele uhradit všechny použitelné daně.</span><span class="sxs-lookup"><span data-stu-id="f06a2-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="f06a2-128">Další informace o cenách specifických pro země (například pro vyrovnání nadcházejících daní) najdete v tématu [plány a ceny pro komerční nabídky na webu Marketplace](https://docs.microsoft.com/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="f06a2-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](https://docs.microsoft.com/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Zobrazuje pracovní postup pro scénář vydaných procesů C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="f06a2-130">Cizí Vydavatel překládá se zákazníkem v USA.</span><span class="sxs-lookup"><span data-stu-id="f06a2-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="f06a2-131">**Scénář D** – všichni cizí vydavatelé (jak je definovala informace o daňovém profilu partnerského centra) v zemích bez smlouvy US (viz [scénář E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) prodej k zákazníkovi na bázi USA (jak je definováno adresou zákaznického účtu).</span><span class="sxs-lookup"><span data-stu-id="f06a2-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="f06a2-132">Státní správa USA vyžaduje, aby se za vydavatele jménem Microsoftu srážková daň.</span><span class="sxs-lookup"><span data-stu-id="f06a2-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="f06a2-133">Daň sražená z výběrů do vydavatele se vypočítá na základě ceny nabídky.</span><span class="sxs-lookup"><span data-stu-id="f06a2-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Zobrazuje pracovní postup pro scénář vypsání procesu D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="f06a2-135">Cizí Vydavatel se smlouvou přepracuje se zákazníkem v USA.</span><span class="sxs-lookup"><span data-stu-id="f06a2-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="f06a2-136">**Scénář E** – všichni zahraniční vydavatelé (jak je definovala informace o daňovém profilu partnerského centra) v zemích se SMLOUVou US, která provádí prodej na zákazníky na bázi USA (jak je definováno adresou zákaznického účtu).</span><span class="sxs-lookup"><span data-stu-id="f06a2-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="f06a2-137">Státní správa USA nepožaduje od Microsoftu srážku daně jménem vydavatele.</span><span class="sxs-lookup"><span data-stu-id="f06a2-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Zobrazuje pracovní postup pro scénář vypsání procesu E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="f06a2-139">Cizí Vydavatel prodává zákazníka, který je registrovaný v EU, v zemi spravované společností Microsoft (mimo Irsko).</span><span class="sxs-lookup"><span data-stu-id="f06a2-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="f06a2-140">**Scénář F** – všechny transakce mezi cizími vydavateli a zákazníky v EU registrovaných DPH (mimo Irsko) ve Microsoft-Managed zemi.</span><span class="sxs-lookup"><span data-stu-id="f06a2-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="f06a2-141">Zákazník neplatí daň na prodej.</span><span class="sxs-lookup"><span data-stu-id="f06a2-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Zobrazuje pracovní postup pro scénář pro výběr procesu F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="f06a2-143">Cizí Vydavatel prodává zákazníka, který je registrovaný v EU, v zemi spravované společností Microsoft (v Irsku).</span><span class="sxs-lookup"><span data-stu-id="f06a2-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="f06a2-144">**Scénář G** – všechny transakce mezi cizími vydavateli a zákazníky v EU registrovaných DPH (v Irsku) ve Microsoft-Managed zemi.</span><span class="sxs-lookup"><span data-stu-id="f06a2-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="f06a2-145">Zákazník zaplatí irskou DPH a společnost Microsoft tuto daň vyplatí pro vládu irské vlády.</span><span class="sxs-lookup"><span data-stu-id="f06a2-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Zobrazuje pracovní postup pro scénář vydaných procesů G.":::

## <a name="next-steps"></a><span data-ttu-id="f06a2-147">Další kroky</span><span class="sxs-lookup"><span data-stu-id="f06a2-147">Next steps</span></span>

- [<span data-ttu-id="f06a2-148">Nejčastější dotazy k vydavateli</span><span class="sxs-lookup"><span data-stu-id="f06a2-148">Publisher FAQ</span></span>](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="f06a2-149">Pokyny k vytvoření platebních a daňových profilů</span><span class="sxs-lookup"><span data-stu-id="f06a2-149">Instructions to create payment and tax profiles</span></span>](https://docs.microsoft.com/partner-center/set-up-your-payout-account?context=/azure/marketplace/context/context#create-a-payment-profile)
