---
title: Oznámení z dubna 2021
description: Oznámení z dubna 2021 pro microsoft Partnerské centrum, včetně nových možností, propagačních akcí, nabídek, trhů nebo změn stávajících nabídek.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 13b8ec9ddd82b38a265606809b8c39c07436e548
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150127"
---
# <a name="april-2021-announcements"></a><span data-ttu-id="9f2fa-103">Oznámení z dubna 2021</span><span class="sxs-lookup"><span data-stu-id="9f2fa-103">April 2021 announcements</span></span>

<span data-ttu-id="9f2fa-104">Tato stránka obsahuje oznámení pro Microsoft Partnerské centrum pro duben 2021.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-104">This page provides the announcements for Microsoft Partner Center for April 2021.</span></span>

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a><span data-ttu-id="9f2fa-105">Připravenost: Aktualizované rozhraní API pro ověřování adres zákazníků CSP bude živě k červnu. možnost testování je nyní k dispozici</span><span class="sxs-lookup"><span data-stu-id="9f2fa-105">Readiness: Updated CSP customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="9f2fa-106">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9f2fa-106">Categories</span></span>

- <span data-ttu-id="9f2fa-107">Datum: 30. 4. 2021</span><span class="sxs-lookup"><span data-stu-id="9f2fa-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="9f2fa-108">Připravenost</span><span class="sxs-lookup"><span data-stu-id="9f2fa-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="9f2fa-109">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9f2fa-109">Summary</span></span>

<span data-ttu-id="9f2fa-110">Aby partneři a zákazníci mohli na základě důvěryhodnosti podnikat, vyzveme partnery k otestování změn rozhraní API pro ověřování adres pro všechny země po celém světě.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9f2fa-111">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9f2fa-111">Impacted audience</span></span>

<span data-ttu-id="9f2fa-112">Partneři CSP s přímým vyúčtováním a nepřímí poskytovatelé, kteří vytvářejí nové nebo aktualizují podrobnosti adresy stávajících zákazníků</span><span class="sxs-lookup"><span data-stu-id="9f2fa-112">CSP direct bill partners and indirect providers who create new or update existing customers’ address details</span></span>

### <a name="details"></a><span data-ttu-id="9f2fa-113">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-113">Details</span></span>

<span data-ttu-id="9f2fa-114">Microsoft běží na vztahu důvěryhodnosti.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-114">Microsoft runs on trust.</span></span> <span data-ttu-id="9f2fa-115">Zavázali jsme se poskytovat vyhovující, bezpečnou a zabezpečenou metodu ověřování adres zákazníků pro transakce s předplatným zákazníků v programu CSP.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="9f2fa-116">Od 31. března 2021 jsme zavedli změny rozhraní API pro ověřování adres.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-116">As of March 31, 2021, we have introduced changes to the Validate Address API.</span></span> <span data-ttu-id="9f2fa-117">Zvou partnery k otestování rozhraní API před jeho zahájením na konci června 2021.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-117">We invite partners to test the API prior to the  go-live at the end of June 2021.</span></span> 

<span data-ttu-id="9f2fa-118">Tyto změny mají vliv pouze na rozhraní API pro ověření adresy.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-118">Note that these changes affect the Validate Address API only.</span></span> <span data-ttu-id="9f2fa-119">Na rozhraní API pro vytvoření zákazníka a aktualizaci fakturačního profilu to nebude mít vliv.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-119">Create Customer and Update Billing Profile APIs aren’t affected.</span></span> <span data-ttu-id="9f2fa-120">I když se navrhovaná adresa v současné době nemusí používat s rozhraním API pro vytvoření zákazníka, důrazně se doporučuje.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-120">Although the suggested address doesn’t currently have to be used with the Create Customer API, it’s highly recommended.</span></span>

<span data-ttu-id="9f2fa-121">Odpověď vrátí jednu z následujících stavových zpráv:</span><span class="sxs-lookup"><span data-stu-id="9f2fa-121">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="9f2fa-122">Status</span><span class="sxs-lookup"><span data-stu-id="9f2fa-122">Status</span></span>     | <span data-ttu-id="9f2fa-123">Popis</span><span class="sxs-lookup"><span data-stu-id="9f2fa-123">Description</span></span> |    <span data-ttu-id="9f2fa-124">Počet vrácených navrhovaných adres</span><span class="sxs-lookup"><span data-stu-id="9f2fa-124">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="9f2fa-125">Ověřená expedice</span><span class="sxs-lookup"><span data-stu-id="9f2fa-125">Verified shippable</span></span> | <span data-ttu-id="9f2fa-126">Adresa je ověřená a je možné ji poslat na adresu .</span><span class="sxs-lookup"><span data-stu-id="9f2fa-126">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="9f2fa-127">Jednoduché</span><span class="sxs-lookup"><span data-stu-id="9f2fa-127">Single</span></span> |
|<span data-ttu-id="9f2fa-128">Ověřují</span><span class="sxs-lookup"><span data-stu-id="9f2fa-128">Verified</span></span> | <span data-ttu-id="9f2fa-129">Adresa je ověřena.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-129">Address is verified.</span></span> | <span data-ttu-id="9f2fa-130">Jednoduché</span><span class="sxs-lookup"><span data-stu-id="9f2fa-130">Single</span></span> |
|<span data-ttu-id="9f2fa-131">Je vyžadována interakce</span><span class="sxs-lookup"><span data-stu-id="9f2fa-131">Interaction required</span></span> | <span data-ttu-id="9f2fa-132">Navrhovaná adresa se významně změnila a potřebuje potvrzení uživatele.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-132">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="9f2fa-133">Jednoduché</span><span class="sxs-lookup"><span data-stu-id="9f2fa-133">Single</span></span> |
|<span data-ttu-id="9f2fa-134">Částečně ulice</span><span class="sxs-lookup"><span data-stu-id="9f2fa-134">Street partial</span></span> | <span data-ttu-id="9f2fa-135">Daná ulice v adrese je částečně a potřebuje další informace.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-135">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="9f2fa-136">Více – maximálně tři</span><span class="sxs-lookup"><span data-stu-id="9f2fa-136">Multiple—maximum of three</span></span> |
|<span data-ttu-id="9f2fa-137">Částečně místní</span><span class="sxs-lookup"><span data-stu-id="9f2fa-137">Premises partial</span></span> | <span data-ttu-id="9f2fa-138">Dané prostory (stavební číslo, číslo sady a další) jsou částečné a vyžadují další informace.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-138">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="9f2fa-139">Více – maximálně tři</span><span class="sxs-lookup"><span data-stu-id="9f2fa-139">Multiple—maximum of three</span></span> |
|<span data-ttu-id="9f2fa-140">Několik</span><span class="sxs-lookup"><span data-stu-id="9f2fa-140">Multiple</span></span> | <span data-ttu-id="9f2fa-141">Adresa obsahuje několik polí, která jsou v této adrese částečně (případně i částečně a částečně v ulici).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-141">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="9f2fa-142">Více – maximálně tři</span><span class="sxs-lookup"><span data-stu-id="9f2fa-142">Multiple—maximum of three</span></span> |
|<span data-ttu-id="9f2fa-143">Žádná</span><span class="sxs-lookup"><span data-stu-id="9f2fa-143">None</span></span> | <span data-ttu-id="9f2fa-144">Adresa je nesprávná.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-144">Address is incorrect.</span></span> | <span data-ttu-id="9f2fa-145">Žádná</span><span class="sxs-lookup"><span data-stu-id="9f2fa-145">None</span></span> |
|<span data-ttu-id="9f2fa-146">Není ověřeno.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-146">Not validated</span></span> | <span data-ttu-id="9f2fa-147">Adresu nelze odeslat prostřednictvím procesu ověřování.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-147">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="9f2fa-148">Žádná</span><span class="sxs-lookup"><span data-stu-id="9f2fa-148">None</span></span> |

<span data-ttu-id="9f2fa-149">PSČ US vrátí další čtyři číslice a pomlčku, například 12345-6789.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-149">US post codes will return an additional four digits + hyphen, for example, 12345-6789.</span></span>

### <a name="next-steps"></a><span data-ttu-id="9f2fa-150">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9f2fa-150">Next steps</span></span>

- <span data-ttu-id="9f2fa-151">Podrobnější pokyny najdete v technické dokumentaci a nejčastější dotazy v [kolekci vyhrazených partnerů](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) .</span><span class="sxs-lookup"><span data-stu-id="9f2fa-151">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="9f2fa-152">Připravte se na začlenění změn pomocí rozhraní API partnerského centra a uživatelského prostředí pro web.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-152">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> 
- <span data-ttu-id="9f2fa-153">Sdílejte své ID tenanta izolovaného prostoru s odborníkem na danou problematiku (Ali pískově), abyste mohli začít připravovat aktualizaci.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-153">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span> 
- <span data-ttu-id="9f2fa-154">Pokud používáte řešení v rámci ovládacího panelu (CPV), obraťte se na CPV.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-154">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="9f2fa-155">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9f2fa-155">Questions?</span></span>

<span data-ttu-id="9f2fa-156">Pokud potřebujete podporu pro vaše operace s Microsoftem, obraťte se na svého partnera, který podporuje Yammer, nebo otevřete [žádost o služby](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-156">If you need support for your operations with Microsoft, reach out to your partner support Yammer group or open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a><span data-ttu-id="9f2fa-157">Nové umístění pro dokumentaci Partnerské centrum API Swagger</span><span class="sxs-lookup"><span data-stu-id="9f2fa-157">New location for Partner Center API Swagger documentation</span></span>

### <a name="categories"></a><span data-ttu-id="9f2fa-158">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9f2fa-158">Categories</span></span>

- <span data-ttu-id="9f2fa-159">Datum: 26. 4. 2021</span><span class="sxs-lookup"><span data-stu-id="9f2fa-159">Date: 2021-04-26</span></span>
- <span data-ttu-id="9f2fa-160">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-160">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="9f2fa-161">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9f2fa-161">Summary</span></span>

<span data-ttu-id="9f2fa-162">Partnerské centrum swaggeru s rozhraním API byly migrovány z předchozího webu dokumentace [Swaggeru](https://apidocs.microsoft.com/services/partnercenter) na [nový web dokumentace Swaggeru.](/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="9f2fa-162">Partner Center API Swagger documents have been migrated from the [previous Swagger Documentation site](https://apidocs.microsoft.com/services/partnercenter) to a [new Swagger Documentation site](/rest/api/partner-center-rest/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9f2fa-163">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9f2fa-163">Impacted audience</span></span>

<span data-ttu-id="9f2fa-164">Partneři s přímým vyúčtováním a nepřímí poskytovatelé, kteří se účastní programu Cloud Solution Provider (CSP), kteří používají rozhraní API Partnerské centrum rozhraní API</span><span class="sxs-lookup"><span data-stu-id="9f2fa-164">Direct bill partners and Indirect Providers participating in the Cloud Solution Provider (CSP) program who are using the Partner Center APIs</span></span>

### <a name="details"></a><span data-ttu-id="9f2fa-165">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-165">Details</span></span>

<span data-ttu-id="9f2fa-166">Od 26. dubna 2021 se dokumentace Partnerské centrum API Swaggeru, včetně obsahu rest API, nachází na [novém webu](/rest/api/partner-center-rest/).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-166">As of April 26, 2021 the Partner Center API Swagger documentation, including Rest API content, is located on a [new site](/rest/api/partner-center-rest/).</span></span> <span data-ttu-id="9f2fa-167">Starý web bude po několika týdnech nedostupný.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-167">The old site will be inaccessible after several weeks.</span></span>

### <a name="benefits"></a><span data-ttu-id="9f2fa-168">Výhody</span><span class="sxs-lookup"><span data-stu-id="9f2fa-168">Benefits</span></span>

<span data-ttu-id="9f2fa-169">V Partnerské centrum API Swaggeru najdete funkci **Try It.**</span><span class="sxs-lookup"><span data-stu-id="9f2fa-169">The Partner Center API Swagger documentation will provide a **Try It** function.</span></span> <span data-ttu-id="9f2fa-170">Pokud chcete tuto funkci použít, budete potřebovat bearer token, který můžete vygenerovat pomocí kroků uvedených [v části Partnerské centrum Authentication](/partner-center/develop/partner-center-authentication#app--user-authentication).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-170">To use this function, you’ll need to have a Bearer Token, which you can generate by following the steps listed in [Partner Center Authentication](/partner-center/develop/partner-center-authentication#app--user-authentication).</span></span>

### <a name="next-steps"></a><span data-ttu-id="9f2fa-171">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9f2fa-171">Next steps</span></span>

<span data-ttu-id="9f2fa-172">Sdílejte tyto informace v rámci vaší organizace, aby příslušný tým mohl zkontrolovat a aktualizovat své procesy.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-172">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="9f2fa-173">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9f2fa-173">Questions?</span></span>

<span data-ttu-id="9f2fa-174">Pokud máte dotazy k těmto nabídekm, podívejte se na příslušné komunity Yammeru.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-174">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a><span data-ttu-id="9f2fa-175">Cloud Solution Provider doby vracení softwaru (CSP) a stažení oznámení o vypršení platnosti odkazu</span><span class="sxs-lookup"><span data-stu-id="9f2fa-175">Cloud Solution Provider (CSP) software return period policy and download link expiry notice</span></span>

### <a name="categories"></a><span data-ttu-id="9f2fa-176">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9f2fa-176">Categories</span></span>

- <span data-ttu-id="9f2fa-177">Datum: 21. 4. 2021</span><span class="sxs-lookup"><span data-stu-id="9f2fa-177">Date: 2021-04-21</span></span>
- <span data-ttu-id="9f2fa-178">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-178">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="9f2fa-179">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9f2fa-179">Summary</span></span>

<span data-ttu-id="9f2fa-180">Došlo ke změnám zásad období vracení softwaru CSP a vypršení platnosti odkazu ke stažení.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-180">There are changes to the CSP software return period policy and download link expiry.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9f2fa-181">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9f2fa-181">Impacted audience</span></span>

<span data-ttu-id="9f2fa-182">Partneři, kteří v CSP provádí transakce s nabídkami časově neomezeného softwaru nebo předplatného softwaru</span><span class="sxs-lookup"><span data-stu-id="9f2fa-182">Partners transacting perpetual software or software subscription offers in CSP</span></span>

### <a name="details"></a><span data-ttu-id="9f2fa-183">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-183">Details</span></span>

<span data-ttu-id="9f2fa-184">Všimněte si následujících důležitých oznámení týkajících se nákupů časově neomezeného softwaru a softwarového předplatného prostřednictvím Partnerské centrum:</span><span class="sxs-lookup"><span data-stu-id="9f2fa-184">Note the following important notifications regarding perpetual software and software subscription purchases through Partner Center:</span></span>

#### <a name="software-return-period-policy"></a><span data-ttu-id="9f2fa-185">Zásady období vrácení softwaru</span><span class="sxs-lookup"><span data-stu-id="9f2fa-185">Software return period policy</span></span>

<span data-ttu-id="9f2fa-186">Od 1. června 2021 se doba vrácení softwarových nabídek v PROGRAMU CSP uvedená v programu Smlouva s partnerem Microsoftu (MPA) změní z 60 dnů od data objednávky na 30 dnů od data objednávky.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-186">From June 1, 2021, the return period for software offers in CSP, as stated in the Microsoft Partner Agreement (MPA), will change from 60 days from order date to 30 days from order date.</span></span>

<span data-ttu-id="9f2fa-187">Po odeslání objednávky softwarové nabídky budou mít partneři 30 dnů od data objednávky, aby mohli odeslat jakékoli revize této objednávky:</span><span class="sxs-lookup"><span data-stu-id="9f2fa-187">After an order for a software offer is submitted, partners will have 30 days from the order date to submit any revisions to such order:</span></span>

- <span data-ttu-id="9f2fa-188">Veškerá Trvalá softwarová licence, která se vrátila během 30denní zpáteční lhůty, obdrží plný kredit placené nákupní ceny.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-188">Any perpetual software license returned within the 30-day return period will receive a full credit of the paid purchase price.</span></span>

- <span data-ttu-id="9f2fa-189">Veškerý produkt pro předplatné softwaru vrácený během 30denní zpáteční lhůty obdrží poměrný kredit placené nákupní ceny.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-189">Any software subscription product returned within the 30-day return period will receive a prorated credit of the paid purchase price.</span></span>

<span data-ttu-id="9f2fa-190">Tato zpráva je následná pro naši e-mailovou komunikaci odeslanou od prosince 2020 do dubna 2021 všem partnerům CSP v souvislosti s návratovou dobou a dalšími aktualizacemi aktivace.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-190">This message is a follow-up to our email communications sent on December 2020 and April 2021 to all CSP partners regarding the return period and other updates to the MPA.</span></span> <span data-ttu-id="9f2fa-191">V těchto oznámeních najdete úplné podrobnosti o změnách, které mají vliv na aktivaci.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-191">Refer to those notices for full details regarding changes affecting the MPA.</span></span>

#### <a name="software-download-link-expiry"></a><span data-ttu-id="9f2fa-192">Vypršení platnosti odkazu na stažení softwaru</span><span class="sxs-lookup"><span data-stu-id="9f2fa-192">Software download link expiry</span></span>

<span data-ttu-id="9f2fa-193">Od 3. června 2021 budou odkazy na stažení softwaru pro trvalé nákupy softwaru a softwaru prostřednictvím partnerského centra mít datum vypršení platnosti 5 dní od prvotního stažení.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-193">From June 3, 2021, the software download links for perpetual software and software subscription product purchases through Partner Center will have an expiration date of five days from the initial download.</span></span> <span data-ttu-id="9f2fa-194">Doba platnosti se bude vztahovat na všechny nákupy do 3. června 2021 a taky do 3. června 2021.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-194">The expiry period will apply to all purchases before June 3, 2021, as well as on or after June 3, 2021.</span></span>

### <a name="next-steps"></a><span data-ttu-id="9f2fa-195">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9f2fa-195">Next steps</span></span>

<span data-ttu-id="9f2fa-196">Přečtěte si [Nejčastější dotazy k návratové době CSP a Stáhněte si informace o vypršení platnosti odkazů](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)a informujte všechny příslušné týmy ve vaší organizaci s těmito změnami:</span><span class="sxs-lookup"><span data-stu-id="9f2fa-196">Review the [CSP return period and download link expiry FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), and inform all appropriate teams within your organization of these changes:</span></span>

### <a name="questions"></a><span data-ttu-id="9f2fa-197">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9f2fa-197">Questions?</span></span>

<span data-ttu-id="9f2fa-198">Otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-198">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a><span data-ttu-id="9f2fa-199">Otevřený licenční program: přechod prodejců do programu Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="9f2fa-199">Open Licensing program: Transitioning resellers to the Cloud Solution Provider (CSP) program</span></span>

### <a name="categories"></a><span data-ttu-id="9f2fa-200">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9f2fa-200">Categories</span></span>

- <span data-ttu-id="9f2fa-201">Datum: 2021-04-19</span><span class="sxs-lookup"><span data-stu-id="9f2fa-201">Date: 2021-04-19</span></span>
- <span data-ttu-id="9f2fa-202">Rozšiřte svou firmu</span><span class="sxs-lookup"><span data-stu-id="9f2fa-202">Grow Your Business</span></span>

### <a name="summary"></a><span data-ttu-id="9f2fa-203">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9f2fa-203">Summary</span></span>

<span data-ttu-id="9f2fa-204">Tato komunikace podrobně popisuje, jak připravit změny, které se připravují do programu Open Licensing.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-204">This communication details how to prepare for the changes that are coming soon to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9f2fa-205">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9f2fa-205">Impacted audience</span></span>

<span data-ttu-id="9f2fa-206">CSP a Open License partneři</span><span class="sxs-lookup"><span data-stu-id="9f2fa-206">CSP and Open License partners</span></span>

### <a name="details"></a><span data-ttu-id="9f2fa-207">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-207">Details</span></span>

<span data-ttu-id="9f2fa-208">V 2020 společnost Microsoft [oznámila](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) , že trvalé licence k softwaru budou široce dostupné partnerům a zákazníkům prostřednictvím programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-208">In 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) that perpetual software licenses will be broadly available to partners and customers through the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="9f2fa-209">První milník byl dosažen v lednu 2021, kdy byly k dispozici komerční nabídky s trvalou dostupností softwaru.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-209">The first milestone was reached in January 2021, when commercial perpetual software offers became available.</span></span> <span data-ttu-id="9f2fa-210">Další klíčový milník bude probíhat v červenci 2021, když budou nabídky [veřejného sektoru](https://aka.ms/openlicensepublicsector) k dispozici.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-210">The next key milestone will happen in July 2021, when [public sector](https://aka.ms/openlicensepublicsector) offers become available.</span></span> <span data-ttu-id="9f2fa-211">Také jsme [komunikovali](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) s účinností od 1. ledna 2022, žádného nového nákupu licence k softwaru ani obnovení programu Software Assurance nebo online služby lze provést prostřednictvím Open License programu.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-211">We also [communicated](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) that effective January 1, 2022, no new software license purchases or renewals of Software Assurance or online services can be made through the Open License program.</span></span>

<span data-ttu-id="9f2fa-212">Přechod trvalého softwaru na program CSP v novém komerčním prostředí pomůže partnerům rozšířit příležitosti k nabídce různých řešení a spravovaných služeb.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-212">The transition of perpetual software to the CSP program in the new commerce experience will help partners to expand the opportunities to offer diverse solutions and managed services.</span></span> <span data-ttu-id="9f2fa-213">Tím se také urychlí přechod zákazníků do cloudu.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-213">This will also accelerate customers’ transition to the cloud.</span></span>  <span data-ttu-id="9f2fa-214">Pro zajištění hladkého přechodu pro naše partnery i zákazníky jsme provedli tyto úpravy a materiály, které tuto digitální transformaci urychlují:</span><span class="sxs-lookup"><span data-stu-id="9f2fa-214">To help ensure a smooth transition for both our partners and customers, we’ve made these adjustments and materials to accelerate this digital transformation:</span></span>

#### <a name="april-2021"></a><span data-ttu-id="9f2fa-215">Duben 2021</span><span class="sxs-lookup"><span data-stu-id="9f2fa-215">April 2021</span></span>

<span data-ttu-id="9f2fa-216">[Nyní k](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)dispozici: Open License převodní materiály mezi CSP pro prodejce</span><span class="sxs-lookup"><span data-stu-id="9f2fa-216">[Now available](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Open License-to-CSP transition materials for resellers</span></span>

#### <a name="july-2021"></a><span data-ttu-id="9f2fa-217">Červenec 2021</span><span class="sxs-lookup"><span data-stu-id="9f2fa-217">July 2021</span></span>

##### <a name="csp"></a><span data-ttu-id="9f2fa-218">CSP</span><span class="sxs-lookup"><span data-stu-id="9f2fa-218">CSP</span></span>

- <span data-ttu-id="9f2fa-219">1. července: Časově neomezené softwarové licence dostupné zákazníkům z veřejného sektoru</span><span class="sxs-lookup"><span data-stu-id="9f2fa-219">July 1: Perpetual software licenses available to public sector customers</span></span>

- <span data-ttu-id="9f2fa-220">7. července: Visual Studio pro a získat časově neomezené softwarové licence pro smlouvu Windows dostupné pro všechny segmenty</span><span class="sxs-lookup"><span data-stu-id="9f2fa-220">July 7: Visual Studio Pro and Get Genuine Windows Agreement  perpetual software licenses available to all segments</span></span>

##### <a name="open-value"></a><span data-ttu-id="9f2fa-221">Open Value</span><span class="sxs-lookup"><span data-stu-id="9f2fa-221">Open Value</span></span>

- <span data-ttu-id="9f2fa-222">1. července: Další SKU dostupné v programu Open Value pro vzdělávání a neziskové organizace poskytující podobné nabídky jako Open License program</span><span class="sxs-lookup"><span data-stu-id="9f2fa-222">July 1: Additional SKUs available in the Open Value program for education and nonprofit, providing similar offers to the Open License program</span></span>

##### <a name="open-license"></a><span data-ttu-id="9f2fa-223">Open License</span><span class="sxs-lookup"><span data-stu-id="9f2fa-223">Open License</span></span>

- <span data-ttu-id="9f2fa-224">1. července: Microsoft už nebude spouštět nové nabídky v Open License programu.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-224">July 1: Microsoft will no longer launch new offers in the Open License program.</span></span>

#### <a name="january-2022"></a><span data-ttu-id="9f2fa-225">Leden 2022</span><span class="sxs-lookup"><span data-stu-id="9f2fa-225">January 2022</span></span>

- <span data-ttu-id="9f2fa-226">1. ledna: Prostřednictvím tohoto programu není možné nic nakupovat ani prodlužovat Open License.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-226">January 1: No new purchases or renewals can be made through the Open License program</span></span>

### <a name="next-steps"></a><span data-ttu-id="9f2fa-227">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9f2fa-227">Next steps</span></span>

#### <a name="csp-indirect-providers"></a><span data-ttu-id="9f2fa-228">Nepřímí poskytovatelé CSP</span><span class="sxs-lookup"><span data-stu-id="9f2fa-228">CSP indirect providers</span></span>

<span data-ttu-id="9f2fa-229">Následující měsíce vám pomůžou se Open License programu CSP tím, že se zúčastní akcí komunity partnerů a využijí materiály pro převod mezi partnery Open License-CSP pro prodejce:</span><span class="sxs-lookup"><span data-stu-id="9f2fa-229">Use the coming months to help Open License resellers orient into the CSP program by attending partner community events and using the Open License-to-CSP transition materials for resellers:</span></span>

- <span data-ttu-id="9f2fa-230">[Open License-to-CSP](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)pro prodejce – Přizpůsobitelné prezentace s přehledem, e-mailová šablona, průvodce onboardingem nepřímých prodejců CSP a další materiály, které vám pomůžou při přechodu na vaše prodejce ve velkém měřítku.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-230">[Open License-to-CSP transition materials for resellers](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span></span>

- <span data-ttu-id="9f2fa-231">[Komunitní akce partnerů CSP](https://globalpbocomm.eventbuilder.com/GlobalCSP) hostované oddělením Microsoft Business Operations</span><span class="sxs-lookup"><span data-stu-id="9f2fa-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) hosted by Microsoft Business Operations.</span></span>  <span data-ttu-id="9f2fa-232">Připojte se k různým relacím a seznamte se se základy CSP (Základy CSP) nebo se učte být aktuální a ptejte se na software v PROGRAMU CSP (Q&A Sessions).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-232">Join the various sessions to learn CSP basics (CSP Fundamentals) or stay up to date, and ask questions regarding Software in CSP (Q&A Sessions).</span></span>

- <span data-ttu-id="9f2fa-233">(Připravujeme) Školení zaměřené na nepřímé prodejce CSP hostované v Microsoft Business Operations</span><span class="sxs-lookup"><span data-stu-id="9f2fa-233">(Coming soon) CSP indirect reseller–focused training session hosted by Microsoft Business Operations.</span></span>

#### <a name="open-license-resellers"></a><span data-ttu-id="9f2fa-234">Open License prodejci</span><span class="sxs-lookup"><span data-stu-id="9f2fa-234">Open License resellers</span></span>

- <span data-ttu-id="9f2fa-235">Pokud vaše organizace není v tuto chvíli zaregistrovaná v programu CSP, obraťte se na svého distributora, kde najdete informace o tom, jak začít.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-235">If your organization isn’t currently enrolled in the CSP program, contact your distributor for information on how to get started.</span></span> <span data-ttu-id="9f2fa-236">[Tady](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)se připojte přímo k poskytovateli.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-236">Connect with an indirect provider [here](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span></span>

- <span data-ttu-id="9f2fa-237">Pokud je vaše organizace už zaregistrovaná v programu CSP, další informace o trvalém softwaru v CSP najdete [tady](https://partner.microsoft.com/resources/collection/software-in-csp).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-237">If your organization is already enrolled in the CSP program, learn more about perpetual software in CSP [here](https://partner.microsoft.com/resources/collection/software-in-csp).</span></span>

### <a name="questions"></a><span data-ttu-id="9f2fa-238">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9f2fa-238">Questions?</span></span>

<span data-ttu-id="9f2fa-239">Další otázky k těmto nabídkám najdete v příslušných komunitách Yammeru.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-239">For further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a><span data-ttu-id="9f2fa-240">Nyní Live: Průvodce globální propagační připravenosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-240">Now live: Global promo readiness guide</span></span>

### <a name="categories"></a><span data-ttu-id="9f2fa-241">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9f2fa-241">Categories</span></span>

- <span data-ttu-id="9f2fa-242">Datum: 2021-04-16</span><span class="sxs-lookup"><span data-stu-id="9f2fa-242">Date: 2021-04-16</span></span>
- <span data-ttu-id="9f2fa-243">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-243">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="9f2fa-244">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9f2fa-244">Summary</span></span>

<span data-ttu-id="9f2fa-245">Připravenost na spuštění publikovala nový [Průvodce globální propagační připravenosti](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) v galerii prostředků připravenosti na operace.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-245">Launch Readiness has published a new [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) on the Operations Readiness resource gallery.</span></span> <span data-ttu-id="9f2fa-246">Tato příručka nabízí konsolidované zobrazení všech aktivních [globálních propagačních akcí](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-246">This guide provides a consolidated view of all active [global promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9f2fa-247">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9f2fa-247">Impacted audience</span></span>

<span data-ttu-id="9f2fa-248">Všechny multilicenční partneři (VL), Dynamics ceníků (DPL) a poskytovatelé Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="9f2fa-248">All Volume Licensing (VL), Dynamics Price List (DPL), and Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="9f2fa-249">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-249">Details</span></span>

<span data-ttu-id="9f2fa-250">Partneři Microsoftu sdíleli s námi potřebu získat konsolidované zobrazení všech globálních propagačních akcí s podpůrnými podrobnostmi.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-250">Microsoft partners have shared with us the need to provide a consolidated view of all global promotions with supporting details.</span></span> <span data-ttu-id="9f2fa-251">Chtěli jste mít k dispozici tuto konsolidovanou příručku, která vám pomůže s tím, že všechny dostupné informace budou snadno přístupné v centrálním a praktickém umístění.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-251">You wanted this consolidated guide to help you use promotions with the confidence that all the available information will be readily accessible in a central and convenient location.</span></span>

<span data-ttu-id="9f2fa-252">Od dubna 2021 Microsoft tuto příručku po měsících aktualizuje a bude k dispozici v galerii prostředků připravená globální akce v galerii prostředků připravenosti na operace.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-252">Beginning in April 2021, Microsoft will update this guide on a monthly basis, and it will be available in a dedicated Global Promo Readiness Guide collection in the Operations Readiness resource gallery.</span></span>

<span data-ttu-id="9f2fa-253">Odkazy na tento průvodce budou také zahrnuty v následujících kolekcích:</span><span class="sxs-lookup"><span data-stu-id="9f2fa-253">Links to this guide will also be included in the following collections:</span></span>

- <span data-ttu-id="9f2fa-254">[Spustit kolekci kalendáře](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), která poskytuje centralizované zobrazení nadcházejících změn a spuštění.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-254">[Launch calendar collection](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), which provides a centralized view of upcoming changes and launches.</span></span>

- <span data-ttu-id="9f2fa-255">[Komunitní kolekce](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), které obsahují podpůrné materiály pro naše měsíční hovory, zvýrazňování nadcházejících změn a včasných témat o provozu.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-255">[Community collections](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), which contain supporting materials for our monthly partner calls, highlighting upcoming changes and timely topics of operational interest.</span></span>

- <span data-ttu-id="9f2fa-256">[Partnerské zpravodaje](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), jako je měsíční aktualizace CSP</span><span class="sxs-lookup"><span data-stu-id="9f2fa-256">[Partner newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), such as CSP Monthly Update</span></span>

<span data-ttu-id="9f2fa-257">V rámci měsíčního připomenutí zveřejníme také oznámení partnerského centra s každým novým problémem Průvodce globální propagační akce.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-257">As a monthly reminder, we will also publish a Partner Center announcement with each new issue of the global promo readiness guide.</span></span>

### <a name="next-steps"></a><span data-ttu-id="9f2fa-258">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9f2fa-258">Next steps</span></span>

<span data-ttu-id="9f2fa-259">Na začátku každého měsíce najdete nejnovější [Průvodce globálními propagačními](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) akcemi v [galerii prostředků připravenosti na operace](https://partner.microsoft.com/resources).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-259">At the start of each month, you will find the latest [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources).</span></span>

<span data-ttu-id="9f2fa-260">Podělte se o tyto informace s příslušnými kontakty ve vaší organizaci a dejte nám vědět, jak užitečná je příručka prostřednictvím stránky Bylo to užitečné?</span><span class="sxs-lookup"><span data-stu-id="9f2fa-260">Share this information with the appropriate contacts in your organizations and let us know how helpful the guide is through the “Was this page helpful?”</span></span> <span data-ttu-id="9f2fa-261">na konci každé stránky.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-261">button at the end of each page.</span></span>

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a><span data-ttu-id="9f2fa-262">Aktualizace a připomenutí Cloud Solution Provider (CSP) z dubna</span><span class="sxs-lookup"><span data-stu-id="9f2fa-262">April Cloud Solution Provider (CSP) community update and reminders</span></span>

### <a name="categories"></a><span data-ttu-id="9f2fa-263">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9f2fa-263">Categories</span></span>

- <span data-ttu-id="9f2fa-264">Datum: 16. 4. 2021</span><span class="sxs-lookup"><span data-stu-id="9f2fa-264">Date: 2021-04-16</span></span>
- <span data-ttu-id="9f2fa-265">Komunitní | Pozvánky a připomenutí</span><span class="sxs-lookup"><span data-stu-id="9f2fa-265">Community | Invites and reminders</span></span>

### <a name="summary"></a><span data-ttu-id="9f2fa-266">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9f2fa-266">Summary</span></span>

<span data-ttu-id="9f2fa-267">Komunitní zdroje CSP jsou k dispozici na vyžádání a každý měsíc se aktualizují, abyste byli informováni a připraveni na změnu v programu CSP.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-267">CSP community resources are available on demand and updated monthly to keep you informed and prepared for change in the CSP program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9f2fa-268">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9f2fa-268">Impacted audience</span></span>

<span data-ttu-id="9f2fa-269">Partneři CSP s přímým vyúčtováním a nepřímí poskytovatelé</span><span class="sxs-lookup"><span data-stu-id="9f2fa-269">CSP direct bill partners and indirect providers</span></span>

### <a name="details"></a><span data-ttu-id="9f2fa-270">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-270">Details</span></span>

<span data-ttu-id="9f2fa-271">Tento měsíc prostředky obsahují následující klíčová témata:</span><span class="sxs-lookup"><span data-stu-id="9f2fa-271">This month, the resources include the following key topics:</span></span>

- [<span data-ttu-id="9f2fa-272">Aktualizace vývoje programu CSP a Open License změn programu</span><span class="sxs-lookup"><span data-stu-id="9f2fa-272">Update to CSP program evolution and Open License program changes</span></span>](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [<span data-ttu-id="9f2fa-273">Změny požadavků na onboarding zákazníků CSP v určitých oblastech</span><span class="sxs-lookup"><span data-stu-id="9f2fa-273">Changes to CSP customer onboarding requirements in certain regions</span></span>](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [<span data-ttu-id="9f2fa-274">Nový formát pro novou fakturu ve formátu PDF obchodu v programu CSP</span><span class="sxs-lookup"><span data-stu-id="9f2fa-274">New format for the new commerce PDF invoice in the CSP program</span></span>](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

<span data-ttu-id="9f2fa-275">V [komunitní kolekci CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)najdete:</span><span class="sxs-lookup"><span data-stu-id="9f2fa-275">Within the [CSP community collection](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), you’ll find:</span></span>

- <span data-ttu-id="9f2fa-276">Bulletin [CSP Monthly Update](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)ke stažení, který v snadno čitelném dokumentu agreguje nejnovější oznámení, aktualizace, události a připomenutí CSP.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-276">The downloadable [CSP Monthly Update newsletter](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), which aggregates recent CSP announcements, updates, events, and reminders in an easy-to-read document.</span></span>

- <span data-ttu-id="9f2fa-277">Kalendář [oznámení CSP,](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)který poskytuje zobrazení časové osy nadcházejících změn, které mají vliv na program.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-277">The [CSP Announcement Calendar](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), which provides a timeline view of upcoming changes affecting the program.</span></span>

- <span data-ttu-id="9f2fa-278">Nový kalendář [uvedení produktu na trh,](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)kde si můžete prohlédnout nadcházející uvedení produktu na trh a nabídky.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-278">The new [product launch calendar](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), where you can view upcoming product launches and offers.</span></span>

- <span data-ttu-id="9f2fa-279">[CSP spouští aktualizační prostředky](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) se snadno použitelným obsahem o klíčových provozních změnách.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-279">[CSP launch update resources](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) with easy-to-consume content on key operational changes.</span></span>

- <span data-ttu-id="9f2fa-280">[Aktualizace a připomenutí klíčových](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) témat CSP, která chystá zájem a dotazy</span><span class="sxs-lookup"><span data-stu-id="9f2fa-280">[Refreshers and reminders](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) on key CSP topics receiving interest and queries.</span></span>

#### <a name="csp-community-call-qas"></a><span data-ttu-id="9f2fa-281">CSP Community Call Q&As</span><span class="sxs-lookup"><span data-stu-id="9f2fa-281">CSP Community Call Q&As</span></span>

<span data-ttu-id="9f2fa-282">Community Call Q&As jsou k dispozici, aby vám pomohly s dotazy souvisejícími s nadcházejícími změnami.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span></span> <span data-ttu-id="9f2fa-283">Zaregistrujte se hned&volání komunity CSP, jak se provádí v dubnu, květen a červnu.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-283">Register now for CSP Community Call Q&As that are taking place in April, May, and June.</span></span> <span data-ttu-id="9f2fa-284">Budou se soustředit na nejnovější spuštění, důležité aktualizace a připomenutí.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-284">These will focus on the latest launches, important refreshers, and reminders.</span></span>

<span data-ttu-id="9f2fa-285">[Zaregistrujte se sem](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-285">[Register here](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span></span>

### <a name="next-steps"></a><span data-ttu-id="9f2fa-286">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9f2fa-286">Next steps</span></span>

<span data-ttu-id="9f2fa-287">Projděte si materiály komunity a zaregistrujte se na dotaz&pro komunitu.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-287">Review the community resources and register for the Community Call Q&A.</span></span>

<span data-ttu-id="9f2fa-288">Abyste se ujistili, že získáte maximum z&, přečtěte si obsah komunity na vyžádání a odešlete své dotazy až 48 hodin před voláním.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-288">To ensure that you get the most from the Community Call Q&A, review the on-demand community content and submit your questions up to 48 hours before the call.</span></span>

### <a name="questions"></a><span data-ttu-id="9f2fa-289">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9f2fa-289">Questions?</span></span>

<span data-ttu-id="9f2fa-290">Toto je nejlepší místo pro otázky související se změnami v programu CSP, který představuje měsíční volání&komunity poskytovatele CSP.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-290">The monthly CSP Community Call Q&A is the best place for questions related to changes in the CSP program.</span></span> <span data-ttu-id="9f2fa-291">Každý měsíc si Projděte materiál a odešlete své otázky předem, abychom mohli strávit relaci v tématech, která jsou pro vás nejdůležitější.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-291">Each month, review the material and submit your questions in advance so that we can spend the session on the topics that are most important to you.</span></span>

<span data-ttu-id="9f2fa-292">Pokud chcete získat další informace, obraťte se na [podporu](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-292">For more information, contact [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span></span>

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a><span data-ttu-id="9f2fa-293">Konečné připomenutí: vyřazení získání kvalifikace z května 6, 2021</span><span class="sxs-lookup"><span data-stu-id="9f2fa-293">Final reminder: Deprecation of GET qualification on May 6, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="9f2fa-294">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9f2fa-294">Categories</span></span>

- <span data-ttu-id="9f2fa-295">Datum: 2021-05-04</span><span class="sxs-lookup"><span data-stu-id="9f2fa-295">Date: 2021-05-04</span></span>

- <span data-ttu-id="9f2fa-296">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-296">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9f2fa-297">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9f2fa-297">Impacted audience</span></span>

<span data-ttu-id="9f2fa-298">Partneři, kteří prodávají akademické a neziskové a státní komunitní Cloud (RSZ) prostřednictvím programu Cloud Solution Provider pomocí rozhraní API partnerského centra</span><span class="sxs-lookup"><span data-stu-id="9f2fa-298">Partners selling Academic, Nonprofit, and Government Community Cloud (GCC) offers through the Cloud Solution Provider program using the Partner Center API</span></span>

### <a name="details"></a><span data-ttu-id="9f2fa-299">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-299">Details</span></span>

<span data-ttu-id="9f2fa-300">Toto oznámení je následná vylepšení partnerského centra [vydané v prosinci](./2020-december.md#1).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-300">This announcement is a follow-up to the Partner Center [enhancements released in December](./2020-december.md#1).</span></span> <span data-ttu-id="9f2fa-301">V rámci této verze se nasadila nová rozhraní API GET a POST a v důsledku toho se **stávající kvalifikace Get vyřadí do 6. května 2021**.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-301">As part of that release, new GET and POST Qualifications APIs were deployed and, as a result, **the existing GET qualification will be retired on May 6, 2021**.</span></span> <span data-ttu-id="9f2fa-302">V tuto chvíli se budete muset převést na použití nového rozhraní API pro POST Center.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-302">By that time, you will need to have transitioned to using the new POST Partner Center APIs.</span></span> <span data-ttu-id="9f2fa-303">Nová rozhraní API pro odesílání vám umožní koupit nabídky vzdělávání, zatímco nové rozhraní API pro získání vám umožní koupit předem kvalifikované nabídky a nabídky RSZ.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-303">The new POST APIs will enable you to purchase Education offers, while the new GET APIs will enable you to purchase pre-qualified Nonprofit and GCC offers.</span></span>

### <a name="next-steps"></a><span data-ttu-id="9f2fa-304">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9f2fa-304">Next steps</span></span>

- <span data-ttu-id="9f2fa-305">**Aktualizujte nové rozhraní API** pro úspěšný a včasný přechod.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-305">**Update to the new APIs** for a successful and timely transition.</span></span>

- <span data-ttu-id="9f2fa-306">**Projděte si nové změny a příručka k rozhraní API partnerského centra** v prostředcích připravenosti operací: [vylepšení procesu ověřování zákazníků z partnerského centra](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-306">**Review the new Partner Center API changes and Guide** in the Operations Readiness resources: [Partner Center Education customer validation process enhancements](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span></span>

- <span data-ttu-id="9f2fa-307">Tyto informace můžete sdílet s příslušnými týmy ve vaší organizaci a prodejci, kteří jim pomůžou tyto změny připravit.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-307">Share this information with the appropriate teams within your organization and with your resellers to help them prepare for these changes.</span></span>

### <a name="questions"></a><span data-ttu-id="9f2fa-308">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9f2fa-308">Questions?</span></span>

<span data-ttu-id="9f2fa-309">Pokud máte dotazy související s tímto oznámením, obraťte se na [podporu partnerského centra](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-309">For any questions related to this notification, contact [Partner Center support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span></span>

### <a name="change-log"></a><span data-ttu-id="9f2fa-310">Protokol změn</span><span class="sxs-lookup"><span data-stu-id="9f2fa-310">Change log</span></span>

- <span data-ttu-id="9f2fa-311">4. května 2021: Závěrečné připomenutí nadcházejícího vyněcování kvalifikace GET</span><span class="sxs-lookup"><span data-stu-id="9f2fa-311">May 4, 2021: Final reminder of upcoming deprecation of GET qualification</span></span>

- <span data-ttu-id="9f2fa-312">9. dubna 2021: Připomenutí nadcházejícího vyněcování kvalifikace GET</span><span class="sxs-lookup"><span data-stu-id="9f2fa-312">April 9, 2021: Reminder of upcoming deprecation of GET qualification</span></span> 

- <span data-ttu-id="9f2fa-313">Únor: Aktualizace časových os pro vyněcování kvalifikace GET & PUT</span><span class="sxs-lookup"><span data-stu-id="9f2fa-313">February: Updated timelines for deprecation of GET & PUT qualifications</span></span>

- <span data-ttu-id="9f2fa-314">Leden: Připomenutí nadcházejícího vynětu kvalifikace GET & PUT</span><span class="sxs-lookup"><span data-stu-id="9f2fa-314">January: Reminder of upcoming deprecations of GET & PUT qualifications</span></span>

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a><span data-ttu-id="9f2fa-315">Nový formát pro novou fakturu ve formátu PDF s komerčním obchodováním v CSP</span><span class="sxs-lookup"><span data-stu-id="9f2fa-315">New format for the new commerce PDF invoice in CSP</span></span>

### <a name="categories"></a><span data-ttu-id="9f2fa-316">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9f2fa-316">Categories</span></span>

- <span data-ttu-id="9f2fa-317">Datum: 5. 4. 2021</span><span class="sxs-lookup"><span data-stu-id="9f2fa-317">Date: 2021-04-05</span></span>
- <span data-ttu-id="9f2fa-318">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-318">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="9f2fa-319">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9f2fa-319">Summary</span></span>

<span data-ttu-id="9f2fa-320">Microsoft zavádí nový formát nové faktury za obchod ve formátu PDF v programu Cloud Solution Provider (CSP), aby se místo popisu skladové položky místo podrobností o produktu zobrazují podrobnosti o fakturaci.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-320">Microsoft is introducing a new format for the new commerce PDF invoice in the Cloud Solution Provider (CSP) program to display billing details by product detail instead of SKU description.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9f2fa-321">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9f2fa-321">Impacted audience</span></span>

<span data-ttu-id="9f2fa-322">Partneři, kteří provádí transakce prostřednictvím programu CSP</span><span class="sxs-lookup"><span data-stu-id="9f2fa-322">Partners transacting through the CSP program</span></span>

### <a name="details"></a><span data-ttu-id="9f2fa-323">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-323">Details</span></span>

<span data-ttu-id="9f2fa-324">Od května 2021 microsoft zavádí nový formát nové faktury za obchod ve formátu PDF v programu CSP, aby se místo popisu SKU místo podrobností o produktu zobrazují podrobnosti o fakturaci.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-324">Starting May 2021, Microsoft is introducing a new format for the new commerce PDF invoice in the CSP program to display billing details by product detail instead of SKU description.</span></span> <span data-ttu-id="9f2fa-325">S touto novou aktualizací budeme agregovat řádkové položky podle typu produktu a současně budeme zobrazovat každý produkt na samostatném řádku.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-325">With this new update, we will be aggregating the line items by product type while displaying every product on an individual line.</span></span>

<span data-ttu-id="9f2fa-326">Partneři si všimnou, že se tato změna projeví na své květnové faktuře za fakturační období od 1. dubna 2021 do 30. dubna 2021.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-326">Partners will notice this change coming into effect in their May invoice for the billing period between April 1, 2021 and April 30, 2021.</span></span> <span data-ttu-id="9f2fa-327">Ovlivněné nabídky jsou Microsoft Azure instance, předplatná Azure (plán Azure) a Marketplace.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-327">The affected offers are Microsoft Azure Reserved Instance, Azure subscriptions (Azure plan), and Marketplace.</span></span>

<span data-ttu-id="9f2fa-328">Všechny žádosti o opětovné vystavení kreditu provedené po aktualizaci formátu faktury se vygenerují v novém formátu.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-328">Any credit-rebill requests made after the invoice format has been updated will be generated in the new format.</span></span>

#### <a name="partner-benefits"></a><span data-ttu-id="9f2fa-329">Partnerské výhody</span><span class="sxs-lookup"><span data-stu-id="9f2fa-329">Partner benefits</span></span>

<span data-ttu-id="9f2fa-330">Tato aktualizace nabídne partnerům následující vylepšení možností fakturace:</span><span class="sxs-lookup"><span data-stu-id="9f2fa-330">This update will offer the following improvements to the invoicing experience for partners:</span></span>

- <span data-ttu-id="9f2fa-331">Snížení velikosti faktury při zachování důležitých dat</span><span class="sxs-lookup"><span data-stu-id="9f2fa-331">Reduced invoice size while retaining critical data</span></span>

- <span data-ttu-id="9f2fa-332">Sladění formátu s oborové standardy pro kompaktní a uživatelsky přívětivé faktury</span><span class="sxs-lookup"><span data-stu-id="9f2fa-332">Alignment of the format to the industry standards for compact and user-friendly invoices</span></span> 

<span data-ttu-id="9f2fa-333">Následující prvky nebudou ovlivněny:</span><span class="sxs-lookup"><span data-stu-id="9f2fa-333">The following elements will not be affected:</span></span>

- <span data-ttu-id="9f2fa-334">Stránka souhrnu fakturace na faktuře VE FORMÁTU PDF</span><span class="sxs-lookup"><span data-stu-id="9f2fa-334">Billing summary page on the invoice PDF</span></span>

- <span data-ttu-id="9f2fa-335">Existující fakturační rozhraní API</span><span class="sxs-lookup"><span data-stu-id="9f2fa-335">Existing invoicing APIs</span></span>

- <span data-ttu-id="9f2fa-336">Soubory pro odsouhlasení (soubory rekognoskaci se dají použít k načítání podrobných dat)</span><span class="sxs-lookup"><span data-stu-id="9f2fa-336">Reconciliation files (Recon files can be used for retrieving granular data.)</span></span> 

- <span data-ttu-id="9f2fa-337">Používání a fakturování poplatků na základě licencí</span><span class="sxs-lookup"><span data-stu-id="9f2fa-337">Usage and license-based charges invoices</span></span>

### <a name="next-steps"></a><span data-ttu-id="9f2fa-338">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9f2fa-338">Next steps</span></span>

<span data-ttu-id="9f2fa-339">Projděte si informace o tomto tématu v [galerii prostředků připravenosti operací](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) na webu Microsoft Partner.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-339">Review the information about this topic in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) on the Microsoft partner website.</span></span> <span data-ttu-id="9f2fa-340">Další informace o fakturačních a daňových tématech, včetně fakturačních prostředků, faktur, fakturace CSP a daní, najdete v [části fakturace](../billing.md) v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-340">For more information about billing and tax topics including billing resources, invoices, CSP billing, and taxes, visit the [Billing section](../billing.md) in Partner Center.</span></span>

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a><span data-ttu-id="9f2fa-341">Změny požadavků na registraci zákazníků poskytovatele Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="9f2fa-341">Changes to the Cloud Solution Provider (CSP) customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="9f2fa-342">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9f2fa-342">Categories</span></span>

- <span data-ttu-id="9f2fa-343">Datum: 2021-04-02</span><span class="sxs-lookup"><span data-stu-id="9f2fa-343">Date: 2021-04-02</span></span>
- <span data-ttu-id="9f2fa-344">Nabídky/trhy</span><span class="sxs-lookup"><span data-stu-id="9f2fa-344">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="9f2fa-345">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9f2fa-345">Summary</span></span>

<span data-ttu-id="9f2fa-346">V rámci našeho závazku pomáhat partnerům a zákazníkům, kteří provozují své podnikání na základě důvěry, budeme požadovat další informace o zákaznících, účinnost 25. března 2021.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-346">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9f2fa-347">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9f2fa-347">Impacted audience</span></span>

<span data-ttu-id="9f2fa-348">Partneři poskytovatele CSP a nepřímá poskytovatelé, kteří mají nové nebo existující zákazníky v zemích uvedených v další části</span><span class="sxs-lookup"><span data-stu-id="9f2fa-348">CSP direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="9f2fa-349">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-349">Details</span></span>

<span data-ttu-id="9f2fa-350">Microsoft běží na důvěryhodnosti.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-350">Microsoft runs on trust.</span></span> <span data-ttu-id="9f2fa-351">Zavázali jsme se poskytovat vyhovující, bezpečné a zabezpečené metody ověřování zákazníků pro transakce předplatných zákazníka v programu CSP.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-351">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="9f2fa-352">25. března 2021 budeme zavádět vylepšení rozhraní API partnerského centra a uživatelského rozhraní, které bude mít vliv na partnery, kteří splňují obě následující kritéria:</span><span class="sxs-lookup"><span data-stu-id="9f2fa-352">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

- <span data-ttu-id="9f2fa-353">Partner má přímý fakturační vztah s Microsoftem (to znamená, že partner je buď přímým partnerem, nebo nepřímým poskytovatelem).</span><span class="sxs-lookup"><span data-stu-id="9f2fa-353">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

- <span data-ttu-id="9f2fa-354">Partner pracuje s novými nebo stávajícími zákazníky v těchto zemích:</span><span class="sxs-lookup"><span data-stu-id="9f2fa-354">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="9f2fa-355">Thajsko</span><span class="sxs-lookup"><span data-stu-id="9f2fa-355">Thailand</span></span>
    - <span data-ttu-id="9f2fa-356">Vietnam</span><span class="sxs-lookup"><span data-stu-id="9f2fa-356">Vietnam</span></span>
    - <span data-ttu-id="9f2fa-357">Turecko</span><span class="sxs-lookup"><span data-stu-id="9f2fa-357">Turkey</span></span>
    - <span data-ttu-id="9f2fa-358">Polsko</span><span class="sxs-lookup"><span data-stu-id="9f2fa-358">Poland</span></span>
    - <span data-ttu-id="9f2fa-359">Jižní Afrika</span><span class="sxs-lookup"><span data-stu-id="9f2fa-359">South Africa</span></span>
    - <span data-ttu-id="9f2fa-360">Indie</span><span class="sxs-lookup"><span data-stu-id="9f2fa-360">India</span></span>
    - <span data-ttu-id="9f2fa-361">Brazílie</span><span class="sxs-lookup"><span data-stu-id="9f2fa-361">Brazil</span></span>
    - <span data-ttu-id="9f2fa-362">Irák</span><span class="sxs-lookup"><span data-stu-id="9f2fa-362">Iraq</span></span>
    - <span data-ttu-id="9f2fa-363">Myanmar</span><span class="sxs-lookup"><span data-stu-id="9f2fa-363">Myanmar</span></span>
    - <span data-ttu-id="9f2fa-364">Jižní Súdán</span><span class="sxs-lookup"><span data-stu-id="9f2fa-364">South Sudan</span></span>
    - <span data-ttu-id="9f2fa-365">Saúdská Arábie</span><span class="sxs-lookup"><span data-stu-id="9f2fa-365">Saudi Arabia</span></span>
    - <span data-ttu-id="9f2fa-366">Spojené arabské emiráty</span><span class="sxs-lookup"><span data-stu-id="9f2fa-366">United Arab Emirates</span></span>
    - <span data-ttu-id="9f2fa-367">Venezuela</span><span class="sxs-lookup"><span data-stu-id="9f2fa-367">Venezuela</span></span>

<span data-ttu-id="9f2fa-368">Partneři, kteří splňují kritéria, budou muset odeslat registrační ID společnosti zákazníka (označované také jako DIČ organizace zákazníka) a telefonní číslo při příští aktualizaci nebo vytvoření předplatného pro daného zákazníka.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-368">Partners who meet the criteria will have to submit a customer's company registration ID (also known as the customer's organization INN) and phone number when they next update or create a subscription for that customer.</span></span> <span data-ttu-id="9f2fa-369">Tito partneři můžou volitelně zadat také druhé jméno zákazníka.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-369">These partners can also enter an optional middle name for the customer.</span></span>

<span data-ttu-id="9f2fa-370">Všimněte si, že při přidání registračního ID vaší společnosti byste měli použít své obchodní daňové ID, nikoli osobní ID zákazníka.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-370">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="9f2fa-371">Partneři, kteří pracují s novými nebo stávajícími zákazníky v následujících zemích, už jsou připojení k předchozí verzi v listopadu 2020.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-371">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="9f2fa-372">Arménie</span><span class="sxs-lookup"><span data-stu-id="9f2fa-372">Armenia</span></span>
- <span data-ttu-id="9f2fa-373">Ázerbájdžán</span><span class="sxs-lookup"><span data-stu-id="9f2fa-373">Azerbaijan</span></span>
- <span data-ttu-id="9f2fa-374">Bělorusko</span><span class="sxs-lookup"><span data-stu-id="9f2fa-374">Belarus</span></span>
- <span data-ttu-id="9f2fa-375">Maďarsko</span><span class="sxs-lookup"><span data-stu-id="9f2fa-375">Hungary</span></span>
- <span data-ttu-id="9f2fa-376">Kazachstán</span><span class="sxs-lookup"><span data-stu-id="9f2fa-376">Kazakhstan</span></span>
- <span data-ttu-id="9f2fa-377">Kyrgyzstán</span><span class="sxs-lookup"><span data-stu-id="9f2fa-377">Kyrgyzstan</span></span>
- <span data-ttu-id="9f2fa-378">Moldavsko</span><span class="sxs-lookup"><span data-stu-id="9f2fa-378">Moldova</span></span>
- <span data-ttu-id="9f2fa-379">Rusko</span><span class="sxs-lookup"><span data-stu-id="9f2fa-379">Russia</span></span>
- <span data-ttu-id="9f2fa-380">Tádžikistán</span><span class="sxs-lookup"><span data-stu-id="9f2fa-380">Tajikistan</span></span>
- <span data-ttu-id="9f2fa-381">Ukrajina</span><span class="sxs-lookup"><span data-stu-id="9f2fa-381">Ukraine</span></span>
- <span data-ttu-id="9f2fa-382">Uzbekistán</span><span class="sxs-lookup"><span data-stu-id="9f2fa-382">Uzbekistan</span></span>

<span data-ttu-id="9f2fa-383">Partneři se zákazníky ve zbytku světa budou mít na konci března 2021 možnost zadat jako volitelné podrobnosti ID registrace společnosti, telefonní číslo a prostřední jméno pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-383">Partners with customers in the rest of the world will have the ability at the end of March 2021 to enter the company registration ID, phone number, and middle name for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="9f2fa-384">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9f2fa-384">Next steps</span></span>

- <span data-ttu-id="9f2fa-385">Podrobnější pokyny najdete v technické dokumentaci [](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) a nejčastějších dotazech ve vyhrazené kolekci partnerů.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-385">Review the technical documentation and frequently asked questions in the dedicated [partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="9f2fa-386">Připravte se na začlenění změn pomocí Partnerské centrum API a webového uživatelského prostředí.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-386">Prepare to incorporate the changes using Partner Center API and web user experience.</span></span> <span data-ttu-id="9f2fa-387">Rozhraní API nebo sdk budou k dispozici pro testování.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-387">API/SDKs will be available for testing.</span></span>
- <span data-ttu-id="9f2fa-388">Nezapomeňte odeslat další data při onboardingu nových zákazníků nebo úpravě stávajících podrobností o zákaznících.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-388">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>
- <span data-ttu-id="9f2fa-389">Pokud používáte řešení dodavatele ovládacích panelů (CPV), obraťte se na svého dodavatele CPV.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-389">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="9f2fa-390">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9f2fa-390">Questions?</span></span>

<span data-ttu-id="9f2fa-391">Pokud máte nějaké dotazy související s ID registrace společnosti (nazývaným také "INN" nebo "TIN").</span><span class="sxs-lookup"><span data-stu-id="9f2fa-391">Contact your tax advisor or local tax office if you have any questions related to the company registration ID (also called INN or TIN).</span></span> <span data-ttu-id="9f2fa-392">Microsoft nemůže poskytnout pokyny k daňovým záležitostem.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-392">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="9f2fa-393">Pokud potřebujete podporu k operacím s Microsoftem, otevřete žádost [o služby.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)</span><span class="sxs-lookup"><span data-stu-id="9f2fa-393">If you need support with your operations with Microsoft, open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a><span data-ttu-id="9f2fa-394">Zobrazení nabídek a uvedení produktů pro tento měsíc na trh</span><span class="sxs-lookup"><span data-stu-id="9f2fa-394">View this month’s product launches and offers</span></span>

### <a name="categories"></a><span data-ttu-id="9f2fa-395">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9f2fa-395">Categories</span></span>

- <span data-ttu-id="9f2fa-396">Datum: 1. 4. 2021</span><span class="sxs-lookup"><span data-stu-id="9f2fa-396">Date: 2021-04-01</span></span>
- <span data-ttu-id="9f2fa-397">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-397">Capabilities</span></span>
 
### <a name="summary"></a><span data-ttu-id="9f2fa-398">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9f2fa-398">Summary</span></span>

<span data-ttu-id="9f2fa-399">Kalendář pro uvedení produktu na trh z dubna 2021 je nyní publikován.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-399">The April 2021 product launch calendar is now published.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9f2fa-400">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9f2fa-400">Impacted audience</span></span>

<span data-ttu-id="9f2fa-401">Všichni partneři, kteří provádí transakce prostřednictvím Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="9f2fa-401">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="9f2fa-402">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9f2fa-402">Details</span></span>

<span data-ttu-id="9f2fa-403">Kalendář spuštění produktu z [](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) dubna 2021 je nyní k dispozici v galerii prostředků provozní připravenosti.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-403">The April 2021 [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) is now available in the Operations readiness resource gallery.</span></span> <span data-ttu-id="9f2fa-404">Nadcházející uvedení produktů a nabídek si můžete prohlédnout tady.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-404">View the upcoming product launches and offers here.</span></span>

### <a name="next-steps"></a><span data-ttu-id="9f2fa-405">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9f2fa-405">Next steps</span></span>

<span data-ttu-id="9f2fa-406">Zkontrolujte kalendář [spuštění produktu a](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)podělte se o informace s příslušnými účastníky ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-406">Review the [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), and share the information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="9f2fa-407">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9f2fa-407">Questions?</span></span>

<span data-ttu-id="9f2fa-408">Pokud máte další dotazy k těmto nabídekm, podívejte se na příslušné komunity Yammeru.</span><span class="sxs-lookup"><span data-stu-id="9f2fa-408">For any further questions about these offers, check your relevant Yammer communities.</span></span>