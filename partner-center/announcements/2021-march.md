---
title: Oznámení z března 2021
description: Z března 2021 oznámení pro partnerské Centrum Microsoftu, včetně nových možností, propagačních akcí, nabídek, trhů nebo změn stávajících nabídek.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 17b8082b8a42050892ff434010952d5f91a39431
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328062"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="9b0fc-103">Oznámení z března 2021</span><span class="sxs-lookup"><span data-stu-id="9b0fc-103">March 2021 announcements</span></span>

<span data-ttu-id="9b0fc-104">Tato stránka poskytuje oznámení pro partnerské Centrum Microsoftu na březen 2021.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a><span data-ttu-id="9b0fc-105">Připravenost: změny v rozhraní API pro ověřování adres zákazníka v červnu v provozu poskytovatele Cloud Solution Provider (CSP) možnost testování je teď dostupná.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-105">Readiness: Changes to the Cloud Solution Provider (CSP) customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-106">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-106">Categories</span></span>

- <span data-ttu-id="9b0fc-107">Datum: 2021-04-30</span><span class="sxs-lookup"><span data-stu-id="9b0fc-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="9b0fc-108">Připravenost</span><span class="sxs-lookup"><span data-stu-id="9b0fc-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="9b0fc-109">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9b0fc-109">Summary</span></span>

<span data-ttu-id="9b0fc-110">Abychom svým partnerům a zákazníkům usnadnili provoz na základě důvěry, budeme zvát partnery, aby otestovali změny v rozhraní API pro ověřování adres pro všechny země po celém světě.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-111">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-111">Impacted audience</span></span>

<span data-ttu-id="9b0fc-112">Poskytovatelé služeb CSP Direct účtují a nepřímá zprostředkovatelé, kteří vytvářejí nové nebo aktualizují podrobnosti o adresách zákazníků.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-112">CSP direct bill partners and indirect providers who create new or update existing customers address details.</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-113">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-113">Details</span></span>

<span data-ttu-id="9b0fc-114">Microsoft běží na důvěryhodnosti.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-114">Microsoft runs on trust.</span></span> <span data-ttu-id="9b0fc-115">Pro účely transakce zákaznických předplatných v programu CSP jsme zajistili poskytování kompatibilní, bezpečné a zabezpečené metody ověřování adres zákazníků.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="9b0fc-116">Od 31. března 2021 jsme představili změny v rozhraní API pro ověřování adres, které pozvaní partneři k testování ještě před tím, než budou v provozu změny v červnu 2021.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-116">As of March 31, 2021, we’ve introduced changes to the Validate Address API that we invited partners to test, prior to going live with the changes in June 2021.</span></span>

<span data-ttu-id="9b0fc-117">Změny mají vliv pouze na ověřování adres API.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-117">Changes affect the Validate Address API only.</span></span> <span data-ttu-id="9b0fc-118">Vytváření zákazníků a aktualizace rozhraní API fakturačních profilů nejsou ovlivněny.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-118">Create Customer and Update Billing Profile APIs aren’t impacted.</span></span>

<span data-ttu-id="9b0fc-119">Odpověď vrátí jednu z následujících stavových zpráv:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="9b0fc-120">Status</span><span class="sxs-lookup"><span data-stu-id="9b0fc-120">Status</span></span>     | <span data-ttu-id="9b0fc-121">Popis</span><span class="sxs-lookup"><span data-stu-id="9b0fc-121">Description</span></span> |    <span data-ttu-id="9b0fc-122">Počet vrácených navrhovaných adres</span><span class="sxs-lookup"><span data-stu-id="9b0fc-122">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="9b0fc-123">Ověřené pro přepravce</span><span class="sxs-lookup"><span data-stu-id="9b0fc-123">Verified shippable</span></span> | <span data-ttu-id="9b0fc-124">Adresa je ověřena a může být expedována.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="9b0fc-125">Jednoduché</span><span class="sxs-lookup"><span data-stu-id="9b0fc-125">Single</span></span> |
|<span data-ttu-id="9b0fc-126">Ověřují</span><span class="sxs-lookup"><span data-stu-id="9b0fc-126">Verified</span></span> | <span data-ttu-id="9b0fc-127">Adresa je ověřena.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-127">Address is verified.</span></span> | <span data-ttu-id="9b0fc-128">Jednoduché</span><span class="sxs-lookup"><span data-stu-id="9b0fc-128">Single</span></span> |
|<span data-ttu-id="9b0fc-129">Je vyžadována interakce</span><span class="sxs-lookup"><span data-stu-id="9b0fc-129">Interaction required</span></span> | <span data-ttu-id="9b0fc-130">Navrhovaná adresa se významně změnila a potřebuje potvrzení uživatele.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-130">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="9b0fc-131">Jednoduché</span><span class="sxs-lookup"><span data-stu-id="9b0fc-131">Single</span></span> |
|<span data-ttu-id="9b0fc-132">Částečně ulice</span><span class="sxs-lookup"><span data-stu-id="9b0fc-132">Street partial</span></span> | <span data-ttu-id="9b0fc-133">Daná ulice v adrese je částečně a potřebuje další informace.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="9b0fc-134">Více – maximálně tři</span><span class="sxs-lookup"><span data-stu-id="9b0fc-134">Multiple—maximum of three</span></span> |
|<span data-ttu-id="9b0fc-135">Částečně místní</span><span class="sxs-lookup"><span data-stu-id="9b0fc-135">Premises partial</span></span> | <span data-ttu-id="9b0fc-136">Dané prostory (stavební číslo, číslo sady a další) jsou částečné a vyžadují další informace.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-136">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="9b0fc-137">Více – maximálně tři</span><span class="sxs-lookup"><span data-stu-id="9b0fc-137">Multiple—maximum of three</span></span> |
|<span data-ttu-id="9b0fc-138">Několik</span><span class="sxs-lookup"><span data-stu-id="9b0fc-138">Multiple</span></span> | <span data-ttu-id="9b0fc-139">Adresa obsahuje několik polí, která jsou v této adrese částečně (případně i částečně a částečně v ulici).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-139">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="9b0fc-140">Více – maximálně tři</span><span class="sxs-lookup"><span data-stu-id="9b0fc-140">Multiple—maximum of three</span></span> |
|<span data-ttu-id="9b0fc-141">Žádné</span><span class="sxs-lookup"><span data-stu-id="9b0fc-141">None</span></span> | <span data-ttu-id="9b0fc-142">Adresa je nesprávná.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-142">Address is incorrect.</span></span> | <span data-ttu-id="9b0fc-143">Žádné</span><span class="sxs-lookup"><span data-stu-id="9b0fc-143">None</span></span> |
|<span data-ttu-id="9b0fc-144">Není ověřeno.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-144">Not validated</span></span> | <span data-ttu-id="9b0fc-145">Adresu nelze odeslat prostřednictvím procesu ověřování.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-145">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="9b0fc-146">Žádné</span><span class="sxs-lookup"><span data-stu-id="9b0fc-146">None</span></span> |

<span data-ttu-id="9b0fc-147">PSČ US vrátí další 4 číslice + spojovník – například 12345-6789.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-147">US post codes will return an additional 4 digits + hyphen - for example, 12345-6789.</span></span>

<span data-ttu-id="9b0fc-148">Jakmile je adresa odeslána k ověření prostřednictvím rozhraní API pro ověření adresy, vrátí se následující schéma odpovědi:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-148">Once an address is submitted for validation via the Validate Address API, the following response schema will be returned:</span></span>

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

<span data-ttu-id="9b0fc-149">Podívejte se na tuto ukázkovou odpověď.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-149">Take a look at this sample response.</span></span> <span data-ttu-id="9b0fc-150">Všimněte si, že pro nás odpověď vrátí další příponu se čtyřmi číslicemi, pokud pro PSČ zadáte jenom pět číslic.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-150">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a><span data-ttu-id="9b0fc-151">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-151">Next steps</span></span>

- <span data-ttu-id="9b0fc-152">Sdílejte své ID tenanta izolovaného prostoru s odborníkem na danou problematiku (Ali pískově), abyste mohli začít připravovat aktualizaci.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-152">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="9b0fc-153">Pokud používáte řešení v rámci ovládacího panelu (CPV), obraťte se na CPV.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-153">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="9b0fc-154">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9b0fc-154">Questions?</span></span>

<span data-ttu-id="9b0fc-155">Pokud potřebujete podporu pro vaše operace s Microsoftem, obraťte se na svého partnera, který podporuje skupinu Yammer.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-155">If you need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

### <a name="change-log"></a><span data-ttu-id="9b0fc-156">Protokol změn:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-156">Change log:</span></span>

- <span data-ttu-id="9b0fc-157">31. března 2020: původní publikace</span><span class="sxs-lookup"><span data-stu-id="9b0fc-157">March 31, 2020: Original publication</span></span>

- <span data-ttu-id="9b0fc-158">30. dubna 2021: aktualizace pro ukázkovou odpověď a podrobnosti o PSČ</span><span class="sxs-lookup"><span data-stu-id="9b0fc-158">April 30, 2021: Updates for sample response and Zip code details</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="9b0fc-159">Nové prostředí v centru pro správu Exchange (EAC)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-159">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-160">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-160">Categories</span></span>

- <span data-ttu-id="9b0fc-161">Datum: 2021-03-29</span><span class="sxs-lookup"><span data-stu-id="9b0fc-161">Date: 2021-03-29</span></span>
- <span data-ttu-id="9b0fc-162">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-162">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="9b0fc-163">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9b0fc-163">Summary</span></span>

<span data-ttu-id="9b0fc-164">Od 27. dubna 2021 se v centru pro správu Exchange (EAC) zavádí nové prostředí, které bude zlepšit každodenní efektivitu pro uživatele.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-164">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-165">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-165">Impacted audience</span></span>

<span data-ttu-id="9b0fc-166">Delegovaní správci přistupující k Exchangi prostřednictvím partnerského centra</span><span class="sxs-lookup"><span data-stu-id="9b0fc-166">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-167">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-167">Details</span></span>

<span data-ttu-id="9b0fc-168">Od 27. dubna 2021 budou partneři, kteří se přecházejí na Exchange prostřednictvím partnerského centra, přesměrováni na nový EAC.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-168">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="9b0fc-169">Toto nové prostředí je teď k dispozici ve verzi Preview a správci můžou aktivovat toto prostředí výběrem přepínače v pravém horním rohu v klasickém poli EAC.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-169">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="9b0fc-170">Můžou také přejít k novému poli EAC tím, že vyberou banner "vyzkoušet ho Now", který se zobrazí na všech stránkách.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-170">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="9b0fc-171">Mezi výhody nového pole EAC patří:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-171">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="9b0fc-172">Přidání přehledů, sestav a mechanismů výstrah pro řízení toku pošty – problémy související s.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-172">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="9b0fc-173">Individuální řídicí panely pro zvýšení produktivity.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-173">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="9b0fc-174">K usnadnění navigace v novém prostředí jsou k dispozici videa v části **školení & příručka** na novém prostředí EAC.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-174">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="9b0fc-175">Tyto informace vám poskytnou přehled o tom, jak můžete nový portál nejlépe využít.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-175">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="9b0fc-176">V rámci této změny nebudou klasické prostředí EAC zastaralé.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-176">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="9b0fc-177">Před implementací jakékoli změny se bude předem informovat.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-177">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="9b0fc-178">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-178">Next steps</span></span>

- <span data-ttu-id="9b0fc-179">Projděte si [materiály k tomuto tématu](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), kde můžete zobrazit snímky obrazovky nového prostředí.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-179">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="9b0fc-180">Tyto informace sdílejte s příslušnými zúčastněnými stranami ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-180">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="9b0fc-181">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9b0fc-181">Questions?</span></span>

<span data-ttu-id="9b0fc-182">Jakékoli otázky týkající se těchto změn najdete v příslušných komunitách Yammeru.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-182">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="9b0fc-183">Operace s Microsoftem: Úvod do kalendářního spuštění produktu</span><span class="sxs-lookup"><span data-stu-id="9b0fc-183">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-184">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-184">Categories</span></span>

- <span data-ttu-id="9b0fc-185">Datum: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="9b0fc-185">Date: 2021-03-25</span></span>
- <span data-ttu-id="9b0fc-186">Nabídky | Moderní pracoviště</span><span class="sxs-lookup"><span data-stu-id="9b0fc-186">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="9b0fc-187">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9b0fc-187">Summary</span></span>

<span data-ttu-id="9b0fc-188">V reakci na zpětnou vazbu od partnerů budou operace společnosti Microsoft zjednodušovat komunikaci při spuštění produktu.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-188">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-189">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-189">Impacted audience</span></span>

<span data-ttu-id="9b0fc-190">Partneři poskytovatele Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-190">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-191">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-191">Details</span></span>

<span data-ttu-id="9b0fc-192">Společnost Microsoft se zavazuje nepřetržitě zdokonalit partnerské prostředí.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-192">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="9b0fc-193">Máme vám zpětnou vazbu od vás, že od Microsoftu jste obdrželi příliš mnoho komunikací, včetně duplicitních oznámení o spuštění produktu.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-193">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="9b0fc-194">V reakci na vaši zpětnou vazbu společnost Microsoft zjednodušila možnosti připravenosti na spuštění produktů pro nové a stávající nabídky.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-194">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="9b0fc-195">Teď vám nabízíme měsíční pohled na spuštění produktu, který je publikovaný v galerii prostředků připravenosti na operace.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-195">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="9b0fc-196">Tento měsíční [Náhled spuštění produktu](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) nahradí konkrétní komunikaci na spuštění produktu v galerii prostředků připravenosti na operace a v oznámeních partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-196">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="9b0fc-197">K tomuto [kalendáři](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) můžete také přistupovat z [kolekcí komunit](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [zobrazení kalendáře](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)a [bulletinů CSP](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-197">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="9b0fc-198">Když publikujete kalendář pro spuštění produktu měsíčně s oznámením v galerii prostředků připravenosti na provoz, pošleme vám oznámení.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-198">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="9b0fc-199">Informace týkající se nové a stávající nabídky najdete pořád v protokolech pro náhled ceníku a v protokolech změn ceníku a také v blogu k produktům, licenčních průvodcích a na stránkách pro marketing produktů.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-199">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="9b0fc-200">Tato změna se bude vztahovat na spuštění následujících produktů:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-200">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="9b0fc-201">Místní aplikace Dynamics</span><span class="sxs-lookup"><span data-stu-id="9b0fc-201">Dynamics on-premises</span></span>
- <span data-ttu-id="9b0fc-202">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9b0fc-202">Microsoft 365</span></span>
- <span data-ttu-id="9b0fc-203">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="9b0fc-203">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="9b0fc-204">Windows</span><span class="sxs-lookup"><span data-stu-id="9b0fc-204">Windows</span></span>
- <span data-ttu-id="9b0fc-205">Server</span><span class="sxs-lookup"><span data-stu-id="9b0fc-205">Server</span></span>  
- <span data-ttu-id="9b0fc-206">nástroje</span><span class="sxs-lookup"><span data-stu-id="9b0fc-206">Tools</span></span>
- <span data-ttu-id="9b0fc-207">Týmy a výpovědi</span><span class="sxs-lookup"><span data-stu-id="9b0fc-207">Teams and Telco</span></span>

<span data-ttu-id="9b0fc-208">Budeme dál posílat konkrétní oznámení ke spuštění produktu, které vyžaduje podrobnosti o připravenosti na operace.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-208">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="9b0fc-209">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-209">Next steps</span></span>

<span data-ttu-id="9b0fc-210">Projděte si materiály k tomuto tématu a sdílejte tyto informace s příslušnými zúčastněnými stranami ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-210">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="9b0fc-211">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9b0fc-211">Questions?</span></span>

<span data-ttu-id="9b0fc-212">Další otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-212">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="9b0fc-213">Změny požadavků na registraci zprostředkovatele CSP pro zákazníky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-213">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-214">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-214">Categories</span></span>

- <span data-ttu-id="9b0fc-215">Datum: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="9b0fc-215">Date: 2021-03-25</span></span>
- <span data-ttu-id="9b0fc-216">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-216">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="9b0fc-217">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9b0fc-217">Summary</span></span>

<span data-ttu-id="9b0fc-218">V rámci našeho závazku pomáhat partnerům a zákazníkům, kteří provozují své podnikání na základě důvěry, budeme požadovat další informace o zákaznících, účinnost 25. března 2021.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-218">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-219">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-219">Impacted audience</span></span>

<span data-ttu-id="9b0fc-220">Partneři poskytovatele Cloud Solution Provider (CSP) a nepřímá poskytovatelé, kteří mají nové nebo existující zákazníky v zemích uvedených v další části</span><span class="sxs-lookup"><span data-stu-id="9b0fc-220">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-221">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-221">Details</span></span>

<span data-ttu-id="9b0fc-222">Microsoft běží na důvěryhodnosti.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-222">Microsoft runs on trust.</span></span> <span data-ttu-id="9b0fc-223">Zavázali jsme se poskytovat vyhovující, bezpečné a zabezpečené metody ověřování zákazníků pro transakce předplatných zákazníka v programu CSP.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-223">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="9b0fc-224">25. března 2021 budeme zavádět vylepšení rozhraní API partnerského centra a uživatelského rozhraní, které bude mít vliv na partnery, kteří splňují obě následující kritéria:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-224">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="9b0fc-225">Partner má přímý fakturační vztah s Microsoftem (to znamená, že partner je buď přímým partnerem, nebo nepřímým poskytovatelem).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-225">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="9b0fc-226">Partner pracuje s novými nebo stávajícími zákazníky v těchto zemích:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-226">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="9b0fc-227">Thajsko</span><span class="sxs-lookup"><span data-stu-id="9b0fc-227">Thailand</span></span>
    - <span data-ttu-id="9b0fc-228">Vietnam</span><span class="sxs-lookup"><span data-stu-id="9b0fc-228">Vietnam</span></span>
    - <span data-ttu-id="9b0fc-229">Turecko</span><span class="sxs-lookup"><span data-stu-id="9b0fc-229">Turkey</span></span>
    - <span data-ttu-id="9b0fc-230">Polsko</span><span class="sxs-lookup"><span data-stu-id="9b0fc-230">Poland</span></span>
    - <span data-ttu-id="9b0fc-231">Jižní Afrika</span><span class="sxs-lookup"><span data-stu-id="9b0fc-231">South Africa</span></span>
    - <span data-ttu-id="9b0fc-232">Indie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-232">India</span></span>
    - <span data-ttu-id="9b0fc-233">Brazílie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-233">Brazil</span></span>
    - <span data-ttu-id="9b0fc-234">Irák</span><span class="sxs-lookup"><span data-stu-id="9b0fc-234">Iraq</span></span>
    - <span data-ttu-id="9b0fc-235">Myanmar</span><span class="sxs-lookup"><span data-stu-id="9b0fc-235">Myanmar</span></span>
    - <span data-ttu-id="9b0fc-236">Jižní Súdán</span><span class="sxs-lookup"><span data-stu-id="9b0fc-236">South Sudan</span></span>
    - <span data-ttu-id="9b0fc-237">Saúdská Arábie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-237">Saudi Arabia</span></span>
    - <span data-ttu-id="9b0fc-238">Spojené arabské emiráty</span><span class="sxs-lookup"><span data-stu-id="9b0fc-238">United Arab Emirates</span></span>
    - <span data-ttu-id="9b0fc-239">Venezuela</span><span class="sxs-lookup"><span data-stu-id="9b0fc-239">Venezuela</span></span>

<span data-ttu-id="9b0fc-240">Partneři, kteří splňují kritéria, budou muset odeslat **registrační ID společnosti** zákazníka (označované také jako **DIČ organizace** zákazníka) a **telefonní číslo** , když připojí nové zákazníky nebo změní stávající podrobnosti o zákaznících.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-240">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="9b0fc-241">Tito partneři můžou volitelně zadat také **druhé jméno** zákazníka.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-241">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="9b0fc-242">Všimněte si, že při přidání registračního ID vaší společnosti byste měli použít své obchodní daňové ID, nikoli osobní ID zákazníka.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-242">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="9b0fc-243">Partneři, kteří pracují s novými nebo stávajícími zákazníky v následujících zemích, už jsou připojení k předchozí verzi v listopadu 2020.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-243">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="9b0fc-244">Arménie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-244">Armenia</span></span>
- <span data-ttu-id="9b0fc-245">Ázerbájdžán</span><span class="sxs-lookup"><span data-stu-id="9b0fc-245">Azerbaijan</span></span>
- <span data-ttu-id="9b0fc-246">Bělorusko</span><span class="sxs-lookup"><span data-stu-id="9b0fc-246">Belarus</span></span>
- <span data-ttu-id="9b0fc-247">Maďarsko</span><span class="sxs-lookup"><span data-stu-id="9b0fc-247">Hungary</span></span>
- <span data-ttu-id="9b0fc-248">Kazachstán</span><span class="sxs-lookup"><span data-stu-id="9b0fc-248">Kazakhstan</span></span>
- <span data-ttu-id="9b0fc-249">Kyrgyzstán</span><span class="sxs-lookup"><span data-stu-id="9b0fc-249">Kyrgyzstan</span></span>
- <span data-ttu-id="9b0fc-250">Moldavsko</span><span class="sxs-lookup"><span data-stu-id="9b0fc-250">Moldova</span></span>
- <span data-ttu-id="9b0fc-251">Rusko</span><span class="sxs-lookup"><span data-stu-id="9b0fc-251">Russia</span></span>
- <span data-ttu-id="9b0fc-252">Tádžikistán</span><span class="sxs-lookup"><span data-stu-id="9b0fc-252">Tajikistan</span></span>
- <span data-ttu-id="9b0fc-253">Ukrajina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-253">Ukraine</span></span>
- <span data-ttu-id="9b0fc-254">Uzbekistán</span><span class="sxs-lookup"><span data-stu-id="9b0fc-254">Uzbekistan</span></span>

<span data-ttu-id="9b0fc-255">Partneři se zákazníky ve zbývající části světa budou mít možnost 25. března 2021 pro zadání **ID registrace společnosti**, **telefonního čísla** a **středního jména** pro zákazníky jako volitelné podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-255">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="9b0fc-256">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-256">Next steps</span></span>

- <span data-ttu-id="9b0fc-257">Podrobnější pokyny najdete v technické dokumentaci a nejčastější dotazy v [kolekci vyhrazených partnerů](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) .</span><span class="sxs-lookup"><span data-stu-id="9b0fc-257">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="9b0fc-258">Připravte se na začlenění změn pomocí rozhraní API partnerského centra a uživatelského prostředí pro web.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-258">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="9b0fc-259">Pro testování bude k dispozici rozhraní API/sady SDK.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-259">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="9b0fc-260">Nezapomeňte odeslat další data při připojování nových zákazníků nebo úpravách stávajících informací o zákaznících.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-260">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="9b0fc-261">Pokud používáte řešení v rámci ovládacího panelu (CPV), obraťte se na CPV.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-261">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="9b0fc-262">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9b0fc-262">Questions?</span></span>

<span data-ttu-id="9b0fc-263">Pokud máte dotazy související s platným identifikátorem (označovaným také jako DIČ nebo DIČ), kontaktujte daňového poradce nebo místní finanční kancelář.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-263">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="9b0fc-264">Microsoft nemůže poskytnout pokyny k daňovým aspektům.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-264">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="9b0fc-265">Pokud potřebujete podporu v rámci svých operací s Microsoftem, [otevřete žádost o služby](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-265">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="9b0fc-266">Opravy provedené 1. března 2021, což je trvalá Ceníková cena softwaru</span><span class="sxs-lookup"><span data-stu-id="9b0fc-266">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-267">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-267">Categories</span></span>

- <span data-ttu-id="9b0fc-268">Datum: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="9b0fc-268">Date: 2021-03-23</span></span>
- <span data-ttu-id="9b0fc-269">Nabídky/trhy</span><span class="sxs-lookup"><span data-stu-id="9b0fc-269">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-270">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-270">Impacted audience</span></span>

<span data-ttu-id="9b0fc-271">Nepřímá poskytovatelé a Přímí partneři poskytující transakční transakce s probíhajícím softwarem v programu Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="9b0fc-271">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="9b0fc-272">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-272">Details</span></span>

<span data-ttu-id="9b0fc-273">Ceník pro trvale zpracovaný software zveřejněný 1. března 2021 zahrnoval trhy, které by se tam nemusely nastavovat.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-273">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="9b0fc-274">Ceník trvalého softwaru byl aktualizován 17. března 2021 se opravami.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-274">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="9b0fc-275">Tyto opravy byly platné pouze pro:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-275">These corrections were only applicable to:</span></span>

- <span data-ttu-id="9b0fc-276">ID produktu: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="9b0fc-276">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="9b0fc-277">Název produktu: upgrade Windows 10 Home na verzi pro pro Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="9b0fc-277">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="9b0fc-278">Odebrané nebo nepodporované trhy: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, ČERNOBÍLé, by, BZ, CI, CL, CM, CO, CR, SH, DO, DZ, ES, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, SWEETIQ, JM, JO, KE, KG, KN, KW, KY, KZ, CR, LK, LY, MA, MC, MD, já, MN, M0, , NI,, NP, OM, PA, PE, PH, PK, PR, PY, QA, R, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, G, UY, UZ, VE, VN, BE, ZM, ZW</span><span class="sxs-lookup"><span data-stu-id="9b0fc-278">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="9b0fc-279">Tyto změny se vztahují pouze na výše uvedený produkt.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-279">These changes only apply to the above product.</span></span> <span data-ttu-id="9b0fc-280">Jiné produkty neobsahovaly žádné opravy.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-280">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="9b0fc-281">Další kroky a zdroje informací</span><span class="sxs-lookup"><span data-stu-id="9b0fc-281">Next steps and resources</span></span>

- <span data-ttu-id="9b0fc-282">Partneři, kteří pracují s nezpracovaným softwarem, by si měli stáhnout nejnovější Ceník softwaru s trvalou cenou.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-282">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="9b0fc-283">V části [kódy zemí v oblasti](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) najdete popisné mapování obou zkratek na země.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-283">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> <span data-ttu-id="9b0fc-284">Vydání sady SDK na .NET Standard (v 1.17.0)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-284">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-285">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-285">Categories</span></span>

- <span data-ttu-id="9b0fc-286">Datum: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="9b0fc-286">Date: 2021-03-23</span></span>

- <span data-ttu-id="9b0fc-287">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-287">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-288">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-288">Impacted audience</span></span>

<span data-ttu-id="9b0fc-289">Přímé partnery a nepřímá poskytovatelé, kteří se účastní programu CSP, kteří používají sadu SDK pro partnerských Center.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-289">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-290">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-290">Details</span></span>

<span data-ttu-id="9b0fc-291">Od března 23 2020 můžou partneři začít stahovat verzi [MicrosoftPartnerCenter. NETSDK (galerie NuGet | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)spolu s aktualizovanými [ukázkami](https://github.com/Microsoft/Partner-Center-DotNet-Samples)služby Public partner Center SDK GitHub.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-291">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="9b0fc-292">Tato verze zahrnuje aktualizace následujících metod:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-292">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="9b0fc-293">Audit byl aktualizován: nové typy operací</span><span class="sxs-lookup"><span data-stu-id="9b0fc-293">Audit Updated: New operation types</span></span>

<span data-ttu-id="9b0fc-294">Přidání nových [typů operací](https://docs.microsoft.com/partner-center/develop/auditing-resources) pro znalost, kdy zákazník schválil a ukončil DAP.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-294">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="9b0fc-295">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="9b0fc-295">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="9b0fc-296">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="9b0fc-296">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="9b0fc-297">Audit byl aktualizován: nové typy prostředků a operací</span><span class="sxs-lookup"><span data-stu-id="9b0fc-297">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="9b0fc-298">Přidali jsme nové [typy prostředků a operací](https://docs.microsoft.com/partner-center/develop/auditing-resources) pro podporu scénáře role adresáře zákazníka.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-298">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="9b0fc-299">Nový typ prostředku "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="9b0fc-299">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="9b0fc-300">Typy operací "AddUserMember" a "RemoveUserMember"</span><span class="sxs-lookup"><span data-stu-id="9b0fc-300">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="9b0fc-301">Aktualizace sady SDK u zákaznických účtů</span><span class="sxs-lookup"><span data-stu-id="9b0fc-301">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="9b0fc-302">Podpora pro GET/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span><span class="sxs-lookup"><span data-stu-id="9b0fc-302">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="9b0fc-303">ZÍSKAT/Customers/{Customer-tenant-ID}/Qualifications</span><span class="sxs-lookup"><span data-stu-id="9b0fc-303">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="9b0fc-304">POST/Customers/{customer_id}/Qualifications? Code = {validationCode}</span><span class="sxs-lookup"><span data-stu-id="9b0fc-304">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="9b0fc-305">Další změny</span><span class="sxs-lookup"><span data-stu-id="9b0fc-305">Additional changes</span></span>

<span data-ttu-id="9b0fc-306">V rámci nového obchodu byly zavedeny následující změny, které jsou aktuálně k dispozici pouze partnerům, kteří jsou součástí M365/D365 New Commerce Experience Technical Preview.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-306">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="9b0fc-307">Partneři, kteří nejsou součástí nové verze nástroje Commerce Technical Preview, by neměli poznamenat dopady a měly by být zpětně kompatibilní.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-307">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="9b0fc-308">Změny katalogu:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-308">Catalog Changes:</span></span>

  - <span data-ttu-id="9b0fc-309">ZÍSKAT/Products/{Product-ID}/skus/{SKU-ID}</span><span class="sxs-lookup"><span data-stu-id="9b0fc-309">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="9b0fc-310">Nákup a správa:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-310">Purchase and Manage:</span></span>
  - <span data-ttu-id="9b0fc-311">ZÍSKAT/customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="9b0fc-311">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="9b0fc-312">ZÍSKAT/customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="9b0fc-312">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="9b0fc-313">/Customers/{customerId}/subscriptions/{subscriptionId} opravy</span><span class="sxs-lookup"><span data-stu-id="9b0fc-313">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="9b0fc-314">ZÍSKAT/customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="9b0fc-314">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="9b0fc-315">ZÍSKAT/customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="9b0fc-315">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="9b0fc-316">PŘÍSPĚVEK/customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="9b0fc-316">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="9b0fc-317">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-317">Next Steps</span></span>

- <span data-ttu-id="9b0fc-318">Stáhněte si nejnovější verzi [MicrosoftPartnerCenter. NETSDK (galerie NuGet | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-318">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="9b0fc-319">Stažení a kontrola [ukázek GitHubu](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-319">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="9b0fc-320">Nabídka CSP pro komerční web Marketplace a FY21 CSP pro opravňující nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-320">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-321">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-321">Categories</span></span>

- <span data-ttu-id="9b0fc-322">Datum: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="9b0fc-322">Date: 2021-03-18</span></span>
- <span data-ttu-id="9b0fc-323">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-323">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-324">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-324">Impacted audience</span></span>

<span data-ttu-id="9b0fc-325">Neposkytovatelé nepřímých zprostředkovatelů a přímých partnerů v programu Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="9b0fc-325">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="9b0fc-326">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-326">Details</span></span>

<span data-ttu-id="9b0fc-327">Nepřímá poskytovatelé a přímá Partnerská partneři v programu Cloud Solution Provider můžou prodávat nabídky třetích stran a získat motivaci slev pro každou způsobilou nabídku třetí strany, která je v partnerském centru nebo Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-327">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="9b0fc-328">Motivace bude ve formě rabatu na účtovaných prodejích pro příslušné nabídky a bude **k dispozici do 30. června 2021**.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-328">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="9b0fc-329">Pokračujte v učení o této nabídce komerčního webu Web Marketplace níže a kontaktujte své zákazníky ještě dnes a Identifikujte správné nabídky, které umožní jejich pokračující úspěšnost a digitální transformaci.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-329">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="9b0fc-330">Spolupracujeme s nezávislými výrobci softwaru (ISV) za účelem uvedení nejnovějších řešení IaaS a SaaS na trh pro zákazníky Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-330">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="9b0fc-331">Vydavatelé ISV mají možnost povolit prodej svých nabídek prostřednictvím kanálu Microsoft Partner.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-331">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="9b0fc-332">Naše pobídkové nabídky spadají do dvou kategorií:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-332">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="9b0fc-333">Vyberte SaaS a IaaS nabídky třetích stran pomocí Azure IP spoluprodejního stavu motivovaní.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-333">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="9b0fc-334">SaaS aplikace integrované s týmy nebo aspoň dvě Microsoft 365 kancelářské aplikace, jako je PowerPoint, Word, Excel, Outlook nebo SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-334">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="9b0fc-335">Další kroky a zdroje informací</span><span class="sxs-lookup"><span data-stu-id="9b0fc-335">Next steps and resources</span></span>

- <span data-ttu-id="9b0fc-336">Přečtěte si, jak získat [pobídky partnerských](https://partner.microsoft.com/membership/partner-incentives) webů pro prodej oprávněných aplikací na webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-336">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="9b0fc-337">Nové nabídky se přidávají měsíčně.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-337">New offers are added monthly.</span></span>  
- [<span data-ttu-id="9b0fc-338">Prostředky pro definanční partnery poskytovatele Cloud Solution Provider Direct</span><span class="sxs-lookup"><span data-stu-id="9b0fc-338">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="9b0fc-339">Prostředky pro motivaci nepřímých poskytovatelů Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="9b0fc-339">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="9b0fc-340">Přečtěte si tuto [prezentaci](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) , kde najdete další informace o prodeji komerčních aplikací z webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-340">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="9b0fc-341">Další materiály najdete [tady](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-341">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="9b0fc-342">Prozkoumejte katalog komerčního tržiště v [partnerském centru](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) nebo [Azure Portal](https://ms.portal.azure.com/#home)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-342">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="9b0fc-343">Použití [rozhraní API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) k integraci aplikací do Marketplace vaší společnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-343">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="9b0fc-344">Přihlaste se k nezávislým výrobcům softwaru, se kterým se zajímá vaše podnikání</span><span class="sxs-lookup"><span data-stu-id="9b0fc-344">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="9b0fc-345">Neposkytovatelé nepřímých zprostředkovatelů potřebují integrovat pomocí rozhraní API a prodejců s postupy, na kterých se aplikace prodávají.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-345">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="9b0fc-346">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9b0fc-346">Questions?</span></span>  

<span data-ttu-id="9b0fc-347">V [tomto článku](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) najdete přehled komerčního tržiště v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-347">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="9b0fc-348">Pokud potřebujete další pomoc, můžete vytvořit žádost o podporu v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-348">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="9b0fc-349">Další informace najdete na adrese [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="9b0fc-349">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="9b0fc-350">Power BI Premium nabídky pro pojmenování a požadované aktualizace</span><span class="sxs-lookup"><span data-stu-id="9b0fc-350">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-351">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-351">Categories</span></span>

- <span data-ttu-id="9b0fc-352">Datum: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="9b0fc-352">Date: 2021-03-18</span></span>
- <span data-ttu-id="9b0fc-353">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-353">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="9b0fc-354">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9b0fc-354">Summary</span></span>

<span data-ttu-id="9b0fc-355">Konečný Ceník od 1. dubna 2021 se aktualizuje, aby se zvýšila přesnost na pojmenování a informace o požadavcích pro Power BI Premium pro jednotlivé uživatele.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-356">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-356">Impacted audience</span></span>

<span data-ttu-id="9b0fc-357">Přímý a nepřímý partneři poskytovatele Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-357">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-358">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-358">Details</span></span>

<span data-ttu-id="9b0fc-359">Konečný Ceník od 1. dubna 2021 se aktualizuje, aby se zvýšila přesnost na pojmenování a informace o požadavcích pro Power BI Premium pro jednotlivé uživatele.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-359">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="9b0fc-360">Až do doby, kdy se aktualizuje Poslední ceník, použijte informace v této části, abyste zajistili, že se správně objednal správný produkt.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-360">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="9b0fc-361">Následující podrobnosti obsahují informace o ovlivněné SKU a požadovaných položkách.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-361">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="9b0fc-362">Zobrazované jméno nabídky na 1. březnu Preview ceníku</span><span class="sxs-lookup"><span data-stu-id="9b0fc-362">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="9b0fc-363">Aktualizovaný zobrazovaný název nabídky na 1. dubnu – konečný Ceník</span><span class="sxs-lookup"><span data-stu-id="9b0fc-363">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="9b0fc-364">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-364">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="9b0fc-365">Power BI Premium Add-On na uživatele (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-365">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="9b0fc-366">Power BI Premium pro uživatele Add-On **(Office)** (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-366">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="9b0fc-367">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="9b0fc-367">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="9b0fc-368">Aby si zákazníci mohli koupit tuto nabídku, musí mít některý z následujících požadavků:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-368">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="9b0fc-369">Zobrazované jméno nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-369">Offer display name</span></span> | <span data-ttu-id="9b0fc-370">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-370">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="9b0fc-371">Microsoft 365 E5 (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-371">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="9b0fc-372">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="9b0fc-372">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="9b0fc-373">Microsoft 365 E5 bez audio Conferencing (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-373">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="9b0fc-374">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="9b0fc-374">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="9b0fc-375">Office 365 E5 (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-375">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="9b0fc-376">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="9b0fc-376">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="9b0fc-377">Zkušební verze Office 365 E5 (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-377">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="9b0fc-378">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="9b0fc-378">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="9b0fc-379">Office 365 E5 bez audio Conferencing (ceny za neziskové zaměstnance)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-379">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="9b0fc-380">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="9b0fc-380">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="9b0fc-381">Pro nákup je nutné mít následující nabídku Power BI Premium:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-381">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="9b0fc-382">Zobrazované jméno nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-382">Offer display name</span></span> | <span data-ttu-id="9b0fc-383">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-383">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="9b0fc-384">Power BI Premium Add-On na uživatele (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-384">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="9b0fc-385">ef0b895b-681B-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="9b0fc-385">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="9b0fc-386">Aby si zákazníci mohli koupit tuto nabídku, musí mít tyto předpoklady:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-386">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="9b0fc-387">Zobrazované jméno nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-387">Offer display name</span></span> | <span data-ttu-id="9b0fc-388">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-388">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="9b0fc-389">Power BI Pro (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-389">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="9b0fc-390">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="9b0fc-390">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="9b0fc-391">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-391">Next steps</span></span>

<span data-ttu-id="9b0fc-392">Projděte si materiály k tomuto tématu a sdílejte tyto informace s příslušnými zúčastněnými stranami ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-392">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="9b0fc-393">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9b0fc-393">Questions?</span></span>

<span data-ttu-id="9b0fc-394">Jakékoli otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-394">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> <span data-ttu-id="9b0fc-395">Aktualizace ceny pro Microsoft 365 F3 v březnu</span><span class="sxs-lookup"><span data-stu-id="9b0fc-395">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-396">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-396">Categories</span></span>

- <span data-ttu-id="9b0fc-397">Datum: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="9b0fc-397">Date: 2021-03-16</span></span>
- <span data-ttu-id="9b0fc-398">Nabídky/trhy</span><span class="sxs-lookup"><span data-stu-id="9b0fc-398">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="9b0fc-399">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9b0fc-399">Summary</span></span>

<span data-ttu-id="9b0fc-400">Nesprávná cena z března 2021 byla opravena pro Microsoft 365 F3, British (GBP) a eura (EUR).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-400">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-401">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-401">Impacted audience</span></span>

<span data-ttu-id="9b0fc-402">Partneři kupují Microsoft 365 F3 v GBP nebo EUR v rozmezí od 1. března 2021 v rámci programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-402">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-403">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-403">Details</span></span>

<span data-ttu-id="9b0fc-404">Společnost Microsoft vyřešila nesprávné ceny za Microsoft 365 F3.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-404">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="9b0fc-405">Nesprávné ceny jsou pro GBP a EUR a jenom pro nabídky zakoupené v rozmezí od 1. března 2021.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-405">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="9b0fc-406">Ovlivněné nabídky a měny jsou uvedeny níže.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-406">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="9b0fc-407">Název nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-407">Offer name</span></span> | <span data-ttu-id="9b0fc-408">Měna</span><span class="sxs-lookup"><span data-stu-id="9b0fc-408">Currency</span></span> | <span data-ttu-id="9b0fc-409">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-409">Offer ID</span></span> | <span data-ttu-id="9b0fc-410">ID materiálu</span><span class="sxs-lookup"><span data-stu-id="9b0fc-410">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="9b0fc-411">Microsoft 365 F3 (dobročinný)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-411">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="9b0fc-412">GBP</span><span class="sxs-lookup"><span data-stu-id="9b0fc-412">GBP</span></span> | <span data-ttu-id="9b0fc-413">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="9b0fc-413">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="9b0fc-414">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="9b0fc-414">AAD-11626</span></span> |
| <span data-ttu-id="9b0fc-415">Microsoft 365 F3 (komerční)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-415">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="9b0fc-416">EUR</span><span class="sxs-lookup"><span data-stu-id="9b0fc-416">EUR</span></span>| <span data-ttu-id="9b0fc-417">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="9b0fc-417">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="9b0fc-418">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="9b0fc-418">AAA-89898</span></span> |
 
<span data-ttu-id="9b0fc-419">Licence na březen a duben Preview – základní ceníky byly aktualizovány 16. března 17:00 tichomořského času (běžný čas).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-419">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="9b0fc-420">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-420">Next steps</span></span>

- <span data-ttu-id="9b0fc-421">Partneři by si měli stáhnout aktuální ceníky založené na licencích, a to v březnu i v dubnu Preview. Tyto ceny se v případě potřeby opraví.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-421">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="9b0fc-422">Společnost Microsoft bude kontaktovat dotčené partnery v nadcházejících týdnech prostřednictvím e-mailu, aby jim informovala o dalších krocích souvisejících s opravou ovlivněných transakcí.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-422">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="9b0fc-423">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9b0fc-423">Questions?</span></span>

<span data-ttu-id="9b0fc-424">Jakékoli další otázky vám poskytne příslušné komunity zprostředkovatele CSP pro Yammer.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-424">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="9b0fc-425">Aktualizace názvu právní společnosti prostřednictvím partnerského centra</span><span class="sxs-lookup"><span data-stu-id="9b0fc-425">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-426">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-426">Categories</span></span>

- <span data-ttu-id="9b0fc-427">Datum: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="9b0fc-427">Date: 2021-03-16</span></span>
- <span data-ttu-id="9b0fc-428">Škálování & škály při zvyšování produktivity</span><span class="sxs-lookup"><span data-stu-id="9b0fc-428">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="9b0fc-429">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9b0fc-429">Summary</span></span>

<span data-ttu-id="9b0fc-430">Od března 2021 se partneři Microsoft Partner Network (MPN) a poskytovatelé Cloud Solution Provider (CSP) můžou prostřednictvím partnerského centra aktualizovat svůj zákonný název společnosti.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-430">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-431">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-431">Impacted audience</span></span>

<span data-ttu-id="9b0fc-432">Partneři programu MPN a neposkytovatelé nepřímých poskytovatelů CSP (neplatí pro partnery s přímým účtováním CSP)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-432">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-433">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-433">Details</span></span>

<span data-ttu-id="9b0fc-434">Od března 2021 partneři programu MPN a nepřímý prodej CSP můžou aktualizovat svůj právní název společnosti prostřednictvím partnerského centra v souladu se svým vlastním způsobem.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-434">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="9b0fc-435">S touto novou funkcí už partneři nebudou muset odeslat lístek podpory pro partnerský partner, aby aktualizovali jeho název společnosti.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-435">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="9b0fc-436">Tím se při provádění těchto aktivit uloží značná doba pro partnery.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-436">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="9b0fc-437">Další informace najdete v tématu [aktualizace svého obchodního profilu](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-437">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="9b0fc-438">Ujistěte se, že název společnosti ve vašem oficiálním obchodním profilu není bez pravopisných chyb a zkratek a přesně odpovídá vašim oficiálním registračním záznamům společnosti.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-438">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="9b0fc-439">Další informace o aktualizaci profilu vaší organizace najdete v tématu [ověření profilu vaší organizace](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-439">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="9b0fc-440">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-440">Next steps</span></span>

<span data-ttu-id="9b0fc-441">Tyto informace můžete sdílet v rámci organizace, aby mohl příslušný tým zkontrolovat a aktualizovat své procesy.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-441">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="9b0fc-442">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9b0fc-442">Questions?</span></span>

<span data-ttu-id="9b0fc-443">Jakékoli další otázky vám poskytne příslušné komunity zprostředkovatele CSP pro Yammer.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-443">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="9b0fc-444">Aktualizace pro vývoj programu Cloud Solution Provider (CSP) a Open License změny programu</span><span class="sxs-lookup"><span data-stu-id="9b0fc-444">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-445">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-445">Categories</span></span>

- <span data-ttu-id="9b0fc-446">Datum: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="9b0fc-446">Date: 2021-03-15</span></span>
- <span data-ttu-id="9b0fc-447">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-447">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="9b0fc-448">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9b0fc-448">Summary</span></span>

<span data-ttu-id="9b0fc-449">Nový komerční a veřejný sektor trvalé nabídky softwaru přicházejí do programu Cloud Solution Provider (CSP) spolu se změnami v programu Open Licensing.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-449">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-450">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-450">Impacted audience</span></span>

<span data-ttu-id="9b0fc-451">Komerční distributoři a spravováni prodejci se prodávají prostřednictvím Open License programu a také všichni partneři CSP s podporou trvalého softwaru.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-451">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-452">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-452">Details</span></span>

<span data-ttu-id="9b0fc-453">V září 2020 společnost Microsoft [oznámila](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) řadu kroků v naší cestě k digitální transformaci, aby bylo možné rozšiřovat příležitosti pro partnery v programu CSP, včetně dostupnosti místního softwaru pro partnery.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-453">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="9b0fc-454">Tyto změny umožňují partnerům rozšiřovat svou firmu a rozšířit jejich dosah tím, že využívají licence na software v cloudu, a jejich umístění pro úspěch v dnešním cloudovém světě.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-454">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="9b0fc-455">Umožňují také přechody zákazníků do cloudu a poskytují partnerům potřebnou flexibilitu pro hybridní cloudová prostředí zákazníka.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-455">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="9b0fc-456">V návaznosti na tuto digitální transformaci oznamujeme následující změny:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-456">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="9b0fc-457">1. července 2021: do ceníku Open License programu nebudou přidány žádné nové SKU, produkty ani propagační akce.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-457">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="9b0fc-458">7. července 2021: dvě komerční nabídky, Získejte originální Windows a Visual Studio Professional a nabídky veřejného sektoru (státní, vzdělávací a neziskové – viz [oznámení](./2020-december.md#9)) se přidají do ceníku trvalého softwaru CSP.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-458">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="9b0fc-459">Ceník najdete v části software [nabídky prodej > price & nabízí](https://partnercenter.microsoft.com/pcv/sales) stránku v partnerském centru a bude se v tomto datu znovu publikovat.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-459">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="9b0fc-460">Úplné podrobnosti týkající se vývoje programu CSP a Open License programových změn naleznete v **následujících krocích** níže.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-460">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="9b0fc-461">Další kroky:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-461">Next Steps:</span></span>

- <span data-ttu-id="9b0fc-462">Vývoj programu CSP: Projděte si [Trvalá softwarová řešení v materiálech připravenosti programu Cloud Solution Provider](https://partner.microsoft.com/resources/collection/software-in-csp#/) .</span><span class="sxs-lookup"><span data-stu-id="9b0fc-462">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="9b0fc-463">Pomocí této [mapy připravenosti](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) můžete rychle najít správné informace pro vaši roli.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-463">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="9b0fc-464">Změny Open License programu: Přečtěte si materiály pro [vývoj programu CSP a Open License program změny](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) připravenosti.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-464">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="9b0fc-465">Pomocí této [mapy připravenosti](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) můžete rychle najít správné informace pro vaši roli.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-465">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="9b0fc-466">Dotazy</span><span class="sxs-lookup"><span data-stu-id="9b0fc-466">Questions</span></span>

<span data-ttu-id="9b0fc-467">Jakékoli další otázky vám poskytne příslušné komunity zprostředkovatele CSP pro Yammer.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-467">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="9b0fc-468">Aktualizace na předchozí oznámení: posouzení Premium, doplněk ke Správci dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="9b0fc-468">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-469">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-469">Categories</span></span>

- <span data-ttu-id="9b0fc-470">Datum: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="9b0fc-470">Date: 2021-03-15</span></span>
- <span data-ttu-id="9b0fc-471">Podpora růstu vaší firmy</span><span class="sxs-lookup"><span data-stu-id="9b0fc-471">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="9b0fc-472">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9b0fc-472">Summary</span></span>

<span data-ttu-id="9b0fc-473">Nabídky zkušební verze by neměly být uvedené na ceníku a budou se odeberou.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-473">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-474">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-474">Impacted audience</span></span>

<span data-ttu-id="9b0fc-475">Transakce partnerů prostřednictvím poskytovatele Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="9b0fc-475">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-476">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-476">Details</span></span>

<span data-ttu-id="9b0fc-477">Ceník by neměl být zahrnut do ceníku.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-477">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="9b0fc-478">Ty se odeberou z ceníku 1. května 2021.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-478">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="9b0fc-479">Původní oznámení [najdete tady](./2021-february.md#4).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-479">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="9b0fc-480">Další zdroje informací</span><span class="sxs-lookup"><span data-stu-id="9b0fc-480">Additional resources</span></span>

- [<span data-ttu-id="9b0fc-481">Microsoft 365 zabezpečení E5 a dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="9b0fc-481">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="9b0fc-482">Sestavování a Správa hodnocení v nástroji Microsoft dodržování předpisů – Microsoft 365 dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="9b0fc-482">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="9b0fc-483">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-483">Next steps</span></span>

<span data-ttu-id="9b0fc-484">Projděte si materiály k tomuto tématu a sdílejte tyto informace s příslušnými zúčastněnými stranami ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-484">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="9b0fc-485">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9b0fc-485">Questions?</span></span>

<span data-ttu-id="9b0fc-486">Otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-486">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="9b0fc-487">Migrace řešení od jednoho komerčního partnera (OCP) přejít na trh (GTM) do komerčního tržiště Microsoftu</span><span class="sxs-lookup"><span data-stu-id="9b0fc-487">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-488">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-488">Categories</span></span>

- <span data-ttu-id="9b0fc-489">Datum: 2021-03-12</span><span class="sxs-lookup"><span data-stu-id="9b0fc-489">Date: 2021-03-12</span></span>
- <span data-ttu-id="9b0fc-490">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-490">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="9b0fc-491">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9b0fc-491">Summary</span></span>

<span data-ttu-id="9b0fc-492">Od 29. března 2021 zahájíte práci s omezeným počtem funkcí GTM (komerční partner), které se vztahují k uvedení na trh (OCP).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-492">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="9b0fc-493">Doporučujeme migrovat vaše řešení na komerční tržiště v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-493">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-494">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-494">Impacted audience</span></span>

<span data-ttu-id="9b0fc-495">Organizace, které společně prodávají s řešeními v OCP GTM</span><span class="sxs-lookup"><span data-stu-id="9b0fc-495">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-496">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-496">Details</span></span>

<span data-ttu-id="9b0fc-497">V prosinci 2020 jsme začali cestu od nástroje Microsoft OCP GTM k komerčnímu tržišti Microsoftu v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-497">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="9b0fc-498">Tento přechod rozšiřuje možnosti komerčního tržiště, kde můžete předprezentovat vaše řešení miliony zákazníků, obousměrně sdílet příležitosti s ostatními prodejci Microsoftu a partnerů a společně prodávat inovativní řešení.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-498">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="9b0fc-499">Další milník v přechodu bude uskutečněn 29. března 2021.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-499">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="9b0fc-500">To je, když začnete používat omezené možnosti OCP GTM, přičemž některá pole se stanou jen pro čtení.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-500">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="9b0fc-501">Pokud v současné době spolupracujete s řešeními v OCP GTM, doporučujeme vám migrovat vaše řešení na komerční tržiště, abyste mohli využívat své možnosti a zjednodušili své možnosti publikování.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-501">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="9b0fc-502">Přechod na komerční tržiště poskytuje partnerskému centru primární cíl pro spoluprodejní prostředí pro publikování.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-502">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="9b0fc-503">Je to místo, kde můžete dál rozšiřovat své podnikání propojením vašich řešení s našimi sdílenými zákazníky přes stejné kanály a prostředí v produktu, které používáme pro produkty Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-503">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="9b0fc-504">[Přečtěte si další informace o komerčním tržišti](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-504">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="9b0fc-505">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-505">Next steps</span></span>

- <span data-ttu-id="9b0fc-506">Pokud jste vaše řešení ještě nepřesunuli, postupujte podle pokynů v [Průvodci přechodem](/azure/marketplace/co-sell-solution-migration) nebo si prohlédněte [podrobné výukové video](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) , které vám umožní dokončit všechny migrační aktivity a zahájit publikování vašich řešení na komerčním webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-506">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="9b0fc-507">Otázky týkající se omezeného prostředí funkcí v systému OCP GTM najdete v tématu [Nejčastější dotazy k požadavkům pro publikování na komerčním webu Microsoft Marketplace](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-507">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="9b0fc-508">(Další informace najdete v části "OCP GTM – omezené možnosti od 29. března 2021.")</span><span class="sxs-lookup"><span data-stu-id="9b0fc-508">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="9b0fc-509">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9b0fc-509">Questions?</span></span>

<span data-ttu-id="9b0fc-510">Pokud máte nějaké dotazy nebo potřebujete další informace, obraťte se na [podporu](https://partner.microsoft.com/support/?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="9b0fc-510">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="9b0fc-511">Rozšiřování nového prostředí pro obchod v programu Cloud Solution Provider (CSP) pro Azure na Rusko</span><span class="sxs-lookup"><span data-stu-id="9b0fc-511">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-512">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-512">Categories</span></span>

- <span data-ttu-id="9b0fc-513">Datum: 2021-03-10</span><span class="sxs-lookup"><span data-stu-id="9b0fc-513">Date: 2021-03-10</span></span>
- <span data-ttu-id="9b0fc-514">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-514">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-515">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-515">Impacted audience</span></span>

<span data-ttu-id="9b0fc-516">Všichni partneři v Rusku procházejí v rámci programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-516">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-517">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-517">Details</span></span>

<span data-ttu-id="9b0fc-518">Od března 10 2021 jsme s radostí oznamujeme dostupnost **nového prostředí pro obchodování v CSP pro Azure v Rusku**.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-518">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="9b0fc-519">Toto prostředí zjednodušuje a vylepšuje způsob, jakým zákazníci kupují a využívají služby Azure.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-519">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="9b0fc-520">Poskytne také partnerům v programu CSP konzistentní pohled na ceny Azure napříč prodejními pohyby, ceny za USD pro globální konzistenci, zarovnání data fakturace a přístup k Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-520">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="9b0fc-521">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-521">Next steps</span></span>

<span data-ttu-id="9b0fc-522">K dispozici je několik prostředků, které představují nové prostředí Azure Commerce a poskytují další informace.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-522">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="9b0fc-523">Nejnovější Nejčastější dotazy, balíčky, video a další informace najdete v [galerii prostředků aktualizace programu CSP](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-523">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="9b0fc-524">Licenční klíč softwaru partnerského centra a stažení</span><span class="sxs-lookup"><span data-stu-id="9b0fc-524">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-525">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-525">Categories</span></span>

- <span data-ttu-id="9b0fc-526">Datum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="9b0fc-526">Date: 2021-03-04</span></span>
- <span data-ttu-id="9b0fc-527">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-527">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="9b0fc-528">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9b0fc-528">Summary</span></span>

<span data-ttu-id="9b0fc-529">Funkce pro stažení softwaru partnerského centra a plnění licenčního klíče se znovu nainstalovala.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-529">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-530">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-530">Impacted audience</span></span>

<span data-ttu-id="9b0fc-531">Všichni partneři poskytovatele Cloud Solution Provider (CSP) postupující trvalé a serverové objednávky softwaru prostřednictvím partnerského centra</span><span class="sxs-lookup"><span data-stu-id="9b0fc-531">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-532">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-532">Details</span></span>

<span data-ttu-id="9b0fc-533">V reakci na zpětnou vazbu od partnerů aktualizujeme možnost plnění partnerského centra a získáte software a licenční klíče pro trvalé objednávky softwaru a předplatného serveru.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-533">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="9b0fc-534">Před odstraněním 19. ledna 2021 se obnoví do předchozího stavu.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-534">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="9b0fc-535">(Viz [oznámení](2020-september.md#17).)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-535">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="9b0fc-536">Všimněte si, že licenční klíče softwaru a odkazy ke stažení jsou cenné a vysoce vyhledané – po prostředcích duševního vlastnictví.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-536">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="9b0fc-537">Pokud dojde k úniku, můžou se rychle vyčerpat z jejich aktivačních limitů a způsobit negativní činnost zákazníků a partnerů.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-537">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="9b0fc-538">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-538">Next steps</span></span>

<span data-ttu-id="9b0fc-539">Pokyny k používání a důležité pokyny k distribuci softwarového klíče najdete v následujících zdrojích informací:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-539">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="9b0fc-540">Prodej místního softwaru prostřednictvím programu CSP</span><span class="sxs-lookup"><span data-stu-id="9b0fc-540">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="9b0fc-541">[Průvodce vytvořením nové obchodní příručky pro partnerský](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) software (viz část **pokyny k distribuci softwarových klíčů** )</span><span class="sxs-lookup"><span data-stu-id="9b0fc-541">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="9b0fc-542">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9b0fc-542">Questions?</span></span>

<span data-ttu-id="9b0fc-543">Pokud máte další dotazy k tomuto oznámení, Projděte si příslušné komunity Yammeru.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-543">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="9b0fc-544">Migrace vašich obchodů z partnera Sales Connect (PSC) do partnerského centra</span><span class="sxs-lookup"><span data-stu-id="9b0fc-544">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-545">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-545">Categories</span></span>

- <span data-ttu-id="9b0fc-546">Datum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="9b0fc-546">Date: 2021-03-04</span></span>
- <span data-ttu-id="9b0fc-547">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-547">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="9b0fc-548">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9b0fc-548">Summary</span></span>

<span data-ttu-id="9b0fc-549">Partner Sales Connect (PSC) se přesune k přístupu jen pro čtení od 31. března 2021, proto doporučujeme začít migrovat vaše obchody z PSC do partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-549">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-550">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-550">Impacted audience</span></span>

<span data-ttu-id="9b0fc-551">Partneři s obchody v PBV</span><span class="sxs-lookup"><span data-stu-id="9b0fc-551">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-552">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-552">Details</span></span>

<span data-ttu-id="9b0fc-553">V rámci našeho sdíleného závazku na růst se dá **společně prodávat pomocí Microsoftu** cesta, která se má **zjistit, zajistit vaše odbornost a rozšířit nároky zákazníků** na pozitivní výsledky zákazníků.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-553">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="9b0fc-554">Díky průměrnému obchodování, který je **3,5 časů rychleji** než normální, vám Správa možností společného prodeje v partnerském centru umožní prodávat přes přímé kanály zákazníka, partnera a prodejce Microsoftu a spravovat celý kanál odkazů na jednom místě.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-554">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="9b0fc-555">**PBV** se přesune k **přístupu jen pro čtení** od **31. března 2021**, proto doporučujeme začít přesun do partnerského centra a získat přístup k těmto vylepšením schopností:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-555">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="9b0fc-556">Přesnější **Směrování** všech obchodů, které sdílíte s Microsoftem, s dopravou prodávající na základě typu pomoci, kterou potřebujete.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-556">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="9b0fc-557">**Ověření nároku** na zajištění opravňujícího řešení pro pobídku a pro splnění kritérií programu ISV Connect, které zjednodušují proces schvalování a konečné ověření platnosti (PoE).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-557">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="9b0fc-558">**Bezproblémové uživatelské prostředí** pro správu všech příležitostí společného prodeje a potenciálních zákazníků na jednom místě.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-558">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="9b0fc-559">V partnerském centru jsme také nedávno přidali nové funkce, které vám pomůžou při přesunu:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-559">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="9b0fc-560">Hromadné operace pro společný prodej příležitostí</span><span class="sxs-lookup"><span data-stu-id="9b0fc-560">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="9b0fc-561">[Funkce migrace koupě](../psc-to-pc.md) (viz část věnované **migraci PSC** .)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-561">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="9b0fc-562">S využitím možností společného prodeje v partnerském centru budou mít prodejní týmy víc času na zaměření na Nurturing potenciálních zákazníků a příležitostí, uzavírání obchodů a vytváření trvalých vztahů se zákazníky.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-562">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="9b0fc-563">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-563">Next steps</span></span>

<span data-ttu-id="9b0fc-564">Pomocí [Průvodce přechodem](../psc-to-pc.md) k partnerským centrům vás seznámíte s postupem migrace vašich obchodů z PSC do partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-564">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="9b0fc-565">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9b0fc-565">Questions?</span></span>

<span data-ttu-id="9b0fc-566">Pokud chcete mít další otázky, obraťte se na [podporu](https://partner.microsoft.com/support/?stage=1).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-566">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="9b0fc-567">Nové produkty a nabídky společnosti Microsoft Dynamics 365, které jsou k dispozici od 1. dubna 2021</span><span class="sxs-lookup"><span data-stu-id="9b0fc-567">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-568">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-568">Categories</span></span>

- <span data-ttu-id="9b0fc-569">Datum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="9b0fc-569">Date: 2021-03-04</span></span>
- <span data-ttu-id="9b0fc-570">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-570">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="9b0fc-571">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9b0fc-571">Summary</span></span>

<span data-ttu-id="9b0fc-572">Od 1. dubna 2021 bude Microsoft spouštět několik nových produktů a nabídek pro program poskytovatele Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-572">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-573">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-573">Impacted audience</span></span>

<span data-ttu-id="9b0fc-574">Všechny partnery, kteří se docházejí prostřednictvím programu Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-574">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-575">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-575">Details</span></span>

<span data-ttu-id="9b0fc-576">Od 1. dubna 2021 bude Microsoft spouštět následující nové produkty a nabídky:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-576">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="9b0fc-577">Power BI Premium na uživatele</span><span class="sxs-lookup"><span data-stu-id="9b0fc-577">Power BI Premium Per User</span></span>
- <span data-ttu-id="9b0fc-578">USL a rozšiřování geografických a segmentů zákazníků</span><span class="sxs-lookup"><span data-stu-id="9b0fc-578">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="9b0fc-579">**Power BI Premium na uživatele**</span><span class="sxs-lookup"><span data-stu-id="9b0fc-579">**Power BI Premium Per User**</span></span>

<span data-ttu-id="9b0fc-580">Microsoft bude zavádět první nabídky Power BI Premium pro jednotlivé uživatele.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-580">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="9b0fc-581">Power BI Premium se aktuálně prodává pouze v konstrukci kapacity.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-581">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="9b0fc-582">Power BI Premium pro jednotlivé uživatele poskytuje přístup k funkcím Enterprise business intelligence (BI) a Analytics.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-582">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="9b0fc-583">Flexibilní organizace pro licencování jednotlivých stanic na malé a střední firmy.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-583">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="9b0fc-584">Další informace o této nabídce najdete v [podrobnostech o verzi Power BI](/power-platform-release-plan/2020wave2/power-bi/planned-features) .</span><span class="sxs-lookup"><span data-stu-id="9b0fc-584">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="9b0fc-585">**Podrobnosti nabídky**</span><span class="sxs-lookup"><span data-stu-id="9b0fc-585">**Offer details**</span></span>

<span data-ttu-id="9b0fc-586">Všimněte si, že název nabídky se mírně liší od ceníku ve verzi Preview.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-586">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="9b0fc-587">Název nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-587">Offer name</span></span> | <span data-ttu-id="9b0fc-588">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-588">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="9b0fc-589">Power BI Premium na uživatele</span><span class="sxs-lookup"><span data-stu-id="9b0fc-589">Power BI Premium Per User</span></span> | <span data-ttu-id="9b0fc-590">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="9b0fc-590">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="9b0fc-591">Power BI Premium na uživatele pro vyučujícího</span><span class="sxs-lookup"><span data-stu-id="9b0fc-591">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="9b0fc-592">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="9b0fc-592">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="9b0fc-593">Power BI Premium na uživatele pro studenty</span><span class="sxs-lookup"><span data-stu-id="9b0fc-593">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="9b0fc-594">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="9b0fc-594">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="9b0fc-595">Power BI Premium na uživatele (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-595">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="9b0fc-596">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="9b0fc-596">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="9b0fc-597">Power BI Premium pro uživatele Add-On</span><span class="sxs-lookup"><span data-stu-id="9b0fc-597">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="9b0fc-598">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="9b0fc-598">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="9b0fc-599">Power BI Premium Add-On na uživatele pro vyučující</span><span class="sxs-lookup"><span data-stu-id="9b0fc-599">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="9b0fc-600">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="9b0fc-600">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="9b0fc-601">Power BI Premium Add-On na uživatele pro studenty</span><span class="sxs-lookup"><span data-stu-id="9b0fc-601">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="9b0fc-602">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="9b0fc-602">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="9b0fc-603">Power BI Premium Add-On na uživatele (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-603">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="9b0fc-604">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="9b0fc-604">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="9b0fc-605">**USL a rozšiřování geografických a segmentů zákazníků**</span><span class="sxs-lookup"><span data-stu-id="9b0fc-605">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="9b0fc-606">Jako při spuštění z prosince 2020 se přidávají nabídky hlasu a marketingu pro zákazníky Dynamics 365 za účelem přidání nových zemí a dalších neziskových a vzdělávacích SKU.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-606">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="9b0fc-607">Název nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-607">Offer name</span></span> | <span data-ttu-id="9b0fc-608">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-608">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="9b0fc-609">Dynamics 365 Customer Voice USL (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-609">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="9b0fc-610">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="9b0fc-610">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="9b0fc-611">Dynamics 365 Customer Voice USL pro vyučujícího</span><span class="sxs-lookup"><span data-stu-id="9b0fc-611">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="9b0fc-612">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="9b0fc-612">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="9b0fc-613">Další informace o těchto nabídkách najdete na následujících stránkách:</span><span class="sxs-lookup"><span data-stu-id="9b0fc-613">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="9b0fc-614">Domovská stránka hlasu pro zákaznickou službu Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="9b0fc-614">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="9b0fc-615">Domovská stránka marketingu Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="9b0fc-615">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="9b0fc-616">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-616">Next steps</span></span>

<span data-ttu-id="9b0fc-617">Projděte si materiály k tomuto tématu a sdílejte tyto informace s příslušnými zúčastněnými stranami ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-617">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="9b0fc-618">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9b0fc-618">Questions?</span></span>

<span data-ttu-id="9b0fc-619">Jakékoli otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-619">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="9b0fc-620">Univerzální tisk společnosti Microsoft je nyní k dispozici v některých sadách.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-620">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="9b0fc-621">Kategorie</span><span class="sxs-lookup"><span data-stu-id="9b0fc-621">Categories</span></span>

- <span data-ttu-id="9b0fc-622">Datum: 2021-03-33</span><span class="sxs-lookup"><span data-stu-id="9b0fc-622">Date: 2021-03-33</span></span>
- <span data-ttu-id="9b0fc-623">Možnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-623">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="9b0fc-624">Souhrn</span><span class="sxs-lookup"><span data-stu-id="9b0fc-624">Summary</span></span>

<span data-ttu-id="9b0fc-625">Univerzální tisk společnosti Microsoft bude k dispozici pro transakce v rámci vybraných Microsoft 365ch sad a jako samostatný doplněk od 1. března 2021.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-625">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="9b0fc-626">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="9b0fc-626">Impacted audience</span></span>

<span data-ttu-id="9b0fc-627">Všechny partnery, kteří se docházejí prostřednictvím programu Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="9b0fc-627">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="9b0fc-628">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="9b0fc-628">Details</span></span>

<span data-ttu-id="9b0fc-629">[Univerzální tisk](https://aka.ms/universalprint) je Microsoft 365 tisková služba, která odstraňuje potřebu místních tiskových serverů a umožňuje zařízením s Windows tisk na tiskárnách registrovaných v Azure.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-629">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="9b0fc-630">Bude k dispozici pro Transact od 1. března 2021.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-630">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="9b0fc-631">Pracovní procesy využívají tisk bez ovladačů, zjednodušené zjišťování tiskáren založené na poloze a intuitivní možnosti tisku bez výukové křivky.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-631">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="9b0fc-632">Zařízení, která jsou připojená k Azure Active Directory (Azure AD), používají k bezpečnému tisku existující přihlašovací údaje Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-632">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="9b0fc-633">Správci spravují tisk pomocí Azure Portal a můžou snadno připojit tiskárny s nativní podporou univerzálního tisku.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-633">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="9b0fc-634">Univerzální tisk se dá nasadit s nekompatibilními tiskárnami pomocí softwaru univerzálního tiskového konektoru.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-634">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="9b0fc-635">Univerzální tisk bude při spuštění vyplněn ve Windows E3, a3, E5 a A5 a Microsoft 365 BP, F3, E3, a3, E5 a a5.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-635">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="9b0fc-636">**Podrobnosti nabídky**</span><span class="sxs-lookup"><span data-stu-id="9b0fc-636">**Offer details**</span></span>

<span data-ttu-id="9b0fc-637">Všimněte si, že název nabídky se mírně liší od ceníku ve verzi Preview.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-637">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="9b0fc-638">Název nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-638">Offer name</span></span> | <span data-ttu-id="9b0fc-639">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-639">Offer ID</span></span> | <span data-ttu-id="9b0fc-640">ID materiálu</span><span class="sxs-lookup"><span data-stu-id="9b0fc-640">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="9b0fc-641">Doplněk objemu univerzálního tisku (úlohy 500) – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9b0fc-641">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="9b0fc-642">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="9b0fc-642">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="9b0fc-643">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="9b0fc-643">9BI-00004</span></span>   |
| <span data-ttu-id="9b0fc-644">Doplněk objemu univerzálního tisku (úlohy 500) pro vyučující – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9b0fc-644">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="9b0fc-645">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="9b0fc-645">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="9b0fc-646">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="9b0fc-646">9BK-00004</span></span>   |
| <span data-ttu-id="9b0fc-647">Doplněk objemu univerzálního tisku (úlohy 500) – Windows</span><span class="sxs-lookup"><span data-stu-id="9b0fc-647">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="9b0fc-648">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="9b0fc-648">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="9b0fc-649">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="9b0fc-649">9BI-00002</span></span>   |
| <span data-ttu-id="9b0fc-650">Doplněk objemu univerzálního tisku (úlohy 500) pro vyučujícího – Windows</span><span class="sxs-lookup"><span data-stu-id="9b0fc-650">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="9b0fc-651">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="9b0fc-651">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="9b0fc-652">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="9b0fc-652">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="9b0fc-653">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9b0fc-653">Next steps</span></span>

<span data-ttu-id="9b0fc-654">Seznamte se s ceníkem a s [přehledem univerzálního tisku](/universal-print/fundamentals/universal-print-whatis).</span><span class="sxs-lookup"><span data-stu-id="9b0fc-654">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="9b0fc-655">Tyto informace Sdílejte se všemi odpovídajícími kontakty ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-655">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="9b0fc-656">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="9b0fc-656">Questions?</span></span>

<span data-ttu-id="9b0fc-657">Jakékoli otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.</span><span class="sxs-lookup"><span data-stu-id="9b0fc-657">For any questions about these offers, check your relevant Yammer communities.</span></span>
