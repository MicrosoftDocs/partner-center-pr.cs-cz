---
title: Jak daňové zásady ovlivňují výběr pro Azure Marketplace
description: Přečtěte si, jak daňové zásady ovlivňují výběr pro Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 32c5cda9558aaaeddaf194eb8258ba732e2ac698
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489964"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="d107e-103">Jak daňové zásady ovlivňují výběr pro Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="d107e-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="d107e-104">**Příslušné role**: globální správce | Správce správy uživatelů | Agent správce</span><span class="sxs-lookup"><span data-stu-id="d107e-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="d107e-105">Úvod</span><span class="sxs-lookup"><span data-stu-id="d107e-105">Introduction</span></span>

<span data-ttu-id="d107e-106">Obchod Microsoft Commercial Marketplace má globální dosah.</span><span class="sxs-lookup"><span data-stu-id="d107e-106">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="d107e-107">K transakcím dochází přes hranice a v závislosti na tom, kde se nachází nezávislý výrobce softwaru (ISV) a zákazník, se může lišit finanční důsledky.</span><span class="sxs-lookup"><span data-stu-id="d107e-107">Transactions occur across borders and depending on where the independent software vendor (ISV) and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="d107e-108">Microsoft AppSource a Azure Marketplace k určení země ISV použijte informace o daňovém profilu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="d107e-108">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="d107e-109">K určení země zákazníka buď použijte fakturační údaje zákazníka, nebo pokud je zákazník v EU, používáme dvě různé informace.</span><span class="sxs-lookup"><span data-stu-id="d107e-109">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="d107e-110">Chcete-li lépe porozumět následujícím scénářům, přečtěte si tabulku s [daňovými podrobnostmi](tax-details-marketplace.md) , která ukazuje, zda společnost Microsoft shromažďuje a vyplatí daně jménem vydavatele nebo pokud tato odpovědnost patří vydavateli.</span><span class="sxs-lookup"><span data-stu-id="d107e-110">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="d107e-111">Všechny příklady hodnot prodejů a sazeb daně v tomto tématu jsou pouze pro ilustrativní účely, nikoli pro přesné hodnoty.</span><span class="sxs-lookup"><span data-stu-id="d107e-111">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="d107e-112">Vydavatel funguje v daňové zemi spravované společností Microsoft</span><span class="sxs-lookup"><span data-stu-id="d107e-112">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="d107e-113">**Scénář a** – transakce, které probíhají mezi vydavatelem a zákazníkem v rámci [daňové země spravované společností Microsoft](tax-details-marketplace.md#microsoft-managed-countries).</span><span class="sxs-lookup"><span data-stu-id="d107e-113">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="d107e-114">Tyto transakce budou mít k dispozici přidanou daň v době prodeje a společnost Microsoft odešle tuto daň do příslušné země.</span><span class="sxs-lookup"><span data-stu-id="d107e-114">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="d107e-115">Z výpočtů a výběrů nejsou zadrženy žádné daně, protože jsou daně výhradně.</span><span class="sxs-lookup"><span data-stu-id="d107e-115">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="d107e-116">Podívejte se na [scénář D](#foreign-publisher-transacts-with-us-customer) pro transakce mezi vydavatelem, který není US, a zákazníkem v USA.</span><span class="sxs-lookup"><span data-stu-id="d107e-116">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Zobrazuje pracovní postup pro scénář vydaných procesů A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="d107e-118">Publisher působí v případě daňové země spravované společností Microsoft, kde poplatek za Marketplace je služba zdanitelná.</span><span class="sxs-lookup"><span data-stu-id="d107e-118">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="d107e-119">**Scénář B** – transakce, které probíhají mezi vydavatelem založeným na USA (jak je definoval informace o daňovém profilu partnera), zákazníkovi v daňové zemi spravované společností Microsoft, kde země ukládá daň na poplatek za tržišti (zdanitelná služba).</span><span class="sxs-lookup"><span data-stu-id="d107e-119">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="d107e-120">V tomto scénáři se daň za poplatek za službu Store odečte od výběr vydavatele.</span><span class="sxs-lookup"><span data-stu-id="d107e-120">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Zobrazuje pracovní postup pro scénář vydaných procesů B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="d107e-122">Vydavatel se chová jako daňová země spravovaná vydavatelem</span><span class="sxs-lookup"><span data-stu-id="d107e-122">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="d107e-123">**Scénář C** – transakce prováděné mezi vydavatelem a zákazníkem v daňové zemi spravované vydavatelem, která neukládá srážkovou daň na zákazníky.</span><span class="sxs-lookup"><span data-stu-id="d107e-123">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="d107e-124">Zákazníci platí bez daně v místě prodeje a jedná se o závazek vydavatele uhradit všechny použitelné daně.</span><span class="sxs-lookup"><span data-stu-id="d107e-124">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="d107e-125">Další informace o cenách specifických pro země (například pro vyrovnání nadcházejících daní) najdete v tématu [plány a ceny pro komerční nabídky na webu Marketplace](/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="d107e-125">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Zobrazuje pracovní postup pro scénář vydaných procesů C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="d107e-127">Cizí Vydavatel překládá se zákazníkem v USA.</span><span class="sxs-lookup"><span data-stu-id="d107e-127">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="d107e-128">**Scénář D** – všichni cizí vydavatelé (jak je definovala informace o daňovém profilu partnerského centra) v zemích bez smlouvy US (viz [scénář E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) prodej k zákazníkovi na bázi USA (jak je definováno adresou zákaznického účtu).</span><span class="sxs-lookup"><span data-stu-id="d107e-128">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="d107e-129">Státní správa USA vyžaduje, aby se za vydavatele jménem Microsoftu srážková daň.</span><span class="sxs-lookup"><span data-stu-id="d107e-129">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="d107e-130">Daň sražená z výběrů do vydavatele se vypočítá na základě ceny nabídky.</span><span class="sxs-lookup"><span data-stu-id="d107e-130">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Zobrazuje pracovní postup pro scénář vypsání procesu D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="d107e-132">Cizí Vydavatel se smlouvou přepracuje se zákazníkem v USA.</span><span class="sxs-lookup"><span data-stu-id="d107e-132">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="d107e-133">**Scénář E** – všichni zahraniční vydavatelé (jak je definovala informace o daňovém profilu partnerského centra) v zemích se SMLOUVou US, která provádí prodej na zákazníky na bázi USA (jak je definováno adresou zákaznického účtu).</span><span class="sxs-lookup"><span data-stu-id="d107e-133">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="d107e-134">Státní správa USA nepožaduje od Microsoftu srážku daně jménem vydavatele.</span><span class="sxs-lookup"><span data-stu-id="d107e-134">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Zobrazuje pracovní postup pro scénář vypsání procesu E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="d107e-136">Cizí Vydavatel prodává zákazníka, který je registrovaný v EU, v zemi spravované společností Microsoft (mimo Irsko).</span><span class="sxs-lookup"><span data-stu-id="d107e-136">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="d107e-137">**Scénář F** – všechny transakce mezi cizími vydavateli a daně z přidané hodnoty (DPH), které zákazníci zaregistrovali (mimo Irsko) ve Microsoft-Managed zemi.</span><span class="sxs-lookup"><span data-stu-id="d107e-137">**Scenario F** – All transactions between foreign publishers and EU value-added tax (VAT)-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="d107e-138">Zákazník neplatí daň na prodej.</span><span class="sxs-lookup"><span data-stu-id="d107e-138">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Zobrazuje pracovní postup pro scénář pro výběr procesu F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="d107e-140">Cizí Vydavatel prodává zákazníka, který je registrovaný v EU, v zemi spravované společností Microsoft (v Irsku).</span><span class="sxs-lookup"><span data-stu-id="d107e-140">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="d107e-141">**Scénář G** – všechny transakce mezi cizími vydavateli a zákazníky v EU registrovaných DPH (v Irsku) ve Microsoft-Managed zemi.</span><span class="sxs-lookup"><span data-stu-id="d107e-141">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="d107e-142">Zákazník zaplatí irskou DPH a společnost Microsoft tuto daň vyplatí pro vládu irské vlády.</span><span class="sxs-lookup"><span data-stu-id="d107e-142">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Zobrazuje pracovní postup pro scénář vydaných procesů G.":::

## <a name="next-steps"></a><span data-ttu-id="d107e-144">Další kroky</span><span class="sxs-lookup"><span data-stu-id="d107e-144">Next steps</span></span>

- [<span data-ttu-id="d107e-145">Nejčastější dotazy k vydavateli</span><span class="sxs-lookup"><span data-stu-id="d107e-145">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="d107e-146">Pokyny k vytvoření platebních a daňových profilů</span><span class="sxs-lookup"><span data-stu-id="d107e-146">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)