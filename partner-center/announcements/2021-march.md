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
ms.openlocfilehash: 12954a5f7eafb138794de879a41026ef54c65da7
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374380"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="261af-103">Oznámení z března 2021</span><span class="sxs-lookup"><span data-stu-id="261af-103">March 2021 announcements</span></span>

<span data-ttu-id="261af-104">Tato stránka poskytuje oznámení pro partnerské Centrum Microsoftu na březen 2021.</span><span class="sxs-lookup"><span data-stu-id="261af-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a><span data-ttu-id="261af-105">Aktualizované rozhraní API pro ověřování zákaznických adres poskytovatele CSP je nyní k dispozici pro testování</span><span class="sxs-lookup"><span data-stu-id="261af-105">Updated CSP customer address validation API now available for testing</span></span>

### <a name="categories"></a><span data-ttu-id="261af-106">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-106">Categories</span></span>

- <span data-ttu-id="261af-107">Datum: 2021-03-31</span><span class="sxs-lookup"><span data-stu-id="261af-107">Date: 2021-03-31</span></span>
- <span data-ttu-id="261af-108">Možnosti</span><span class="sxs-lookup"><span data-stu-id="261af-108">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="261af-109">Souhrn</span><span class="sxs-lookup"><span data-stu-id="261af-109">Summary</span></span>

<span data-ttu-id="261af-110">V rámci našeho závazku pomáhat partnerům a zákazníkům, kteří provozují své podnikání na základě důvěry, budeme zvát partneři po celém světě, aby otestovali změny v rozhraní ValidateAddress API.</span><span class="sxs-lookup"><span data-stu-id="261af-110">As part of our commitment to help partners and customers run their business based on trust, we will be inviting partners worldwide to test the changes to the ValidateAddress API.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-111">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-111">Impacted audience</span></span>

<span data-ttu-id="261af-112">Všichni partneři poskytovatele CSP Direct účtují a nepřímá poskytovatelé, kteří vytvářejí nové nebo aktualizují podrobnosti stávajících adres zákazníka</span><span class="sxs-lookup"><span data-stu-id="261af-112">All CSP direct bill partners and indirect providers who create new or update existing customer address details</span></span>

### <a name="details"></a><span data-ttu-id="261af-113">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-113">Details</span></span>

<span data-ttu-id="261af-114">Microsoft běží na důvěryhodnosti.</span><span class="sxs-lookup"><span data-stu-id="261af-114">Microsoft runs on trust.</span></span> <span data-ttu-id="261af-115">Zavázali jsme se poskytovat kompatibilní, bezpečnou a zabezpečenou metodu odesílání ověření zákaznické adresy pro účely transakcí předplatných zákazníků v programu CSP.</span><span class="sxs-lookup"><span data-stu-id="261af-115">We’re committed to providing a compliant, safe, and secure method of submitting customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="261af-116">V dnešní době 31. března 2021 jsme zavedli změny rozhraní ValidateAddress API, které bychom Vás pozvali k testování, před tím, než budete moct začít pracovat se změnami v červnu 2021.</span><span class="sxs-lookup"><span data-stu-id="261af-116">Today, March 31, 2021, we have introduced changes to the ValidateAddress API that we’d like to invite you to test, prior to going live with the changes in June 2021.</span></span> 

<span data-ttu-id="261af-117">Všimněte si, že tyto změny mají vliv pouze na rozhraní ValidateAddress API.</span><span class="sxs-lookup"><span data-stu-id="261af-117">Note that these changes affect the ValidateAddress API only.</span></span> <span data-ttu-id="261af-118">Rozhraní API CreateCustomer a UpdateBillingProfile nejsou ovlivněná.</span><span class="sxs-lookup"><span data-stu-id="261af-118">CreateCustomer and UpdateBillingProfile APIs are not affected.</span></span>

<span data-ttu-id="261af-119">Odpověď vrátí jednu z následujících stavových zpráv:</span><span class="sxs-lookup"><span data-stu-id="261af-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="261af-120">Status</span><span class="sxs-lookup"><span data-stu-id="261af-120">Status</span></span> | <span data-ttu-id="261af-121">Popis</span><span class="sxs-lookup"><span data-stu-id="261af-121">Description</span></span> | <span data-ttu-id="261af-122">Počet vrácených navrhovaných adres</span><span class="sxs-lookup"><span data-stu-id="261af-122">Number of suggested addresses returned</span></span> |
|----------|-------------|-------------------|
| <span data-ttu-id="261af-123">VerifiedShippable</span><span class="sxs-lookup"><span data-stu-id="261af-123">VerifiedShippable</span></span> | <span data-ttu-id="261af-124">Adresa je ověřena a může být expedována.</span><span class="sxs-lookup"><span data-stu-id="261af-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="261af-125">Jednoduché</span><span class="sxs-lookup"><span data-stu-id="261af-125">Single</span></span> |
| <span data-ttu-id="261af-126">Ověřují</span><span class="sxs-lookup"><span data-stu-id="261af-126">Verified</span></span> | <span data-ttu-id="261af-127">Adresa je ověřena.</span><span class="sxs-lookup"><span data-stu-id="261af-127">Address is verified.</span></span> | <span data-ttu-id="261af-128">Jednoduché</span><span class="sxs-lookup"><span data-stu-id="261af-128">Single</span></span> |
| <span data-ttu-id="261af-129">InteractionRequired</span><span class="sxs-lookup"><span data-stu-id="261af-129">InteractionRequired</span></span> | <span data-ttu-id="261af-130">Navrhované adresy byly významně změněny a potřebuje potvrzení uživatele.</span><span class="sxs-lookup"><span data-stu-id="261af-130">Suggested address(es) has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="261af-131">Jednoduché</span><span class="sxs-lookup"><span data-stu-id="261af-131">Single</span></span> |
| <span data-ttu-id="261af-132">StreetPartial</span><span class="sxs-lookup"><span data-stu-id="261af-132">StreetPartial</span></span> | <span data-ttu-id="261af-133">Daná ulice v adrese je částečně a potřebuje další informace.</span><span class="sxs-lookup"><span data-stu-id="261af-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="261af-134">Více – maximálně tři</span><span class="sxs-lookup"><span data-stu-id="261af-134">Multiple—maximum of three</span></span>|
| <span data-ttu-id="261af-135">PremisesPartial</span><span class="sxs-lookup"><span data-stu-id="261af-135">PremisesPartial</span></span> | <span data-ttu-id="261af-136">Daný prostor (stavební číslo, číslo sady atd.) je částečný a potřebuje další informace.</span><span class="sxs-lookup"><span data-stu-id="261af-136">The given premises (building number, suite number, etc.) is partial and needs more info.</span></span> | <span data-ttu-id="261af-137">Více – maximálně tři</span><span class="sxs-lookup"><span data-stu-id="261af-137">Multiple—maximum of three</span></span> |
| <span data-ttu-id="261af-138">Několik</span><span class="sxs-lookup"><span data-stu-id="261af-138">Multiple</span></span> | <span data-ttu-id="261af-139">Adresa obsahuje několik polí, která jsou v této adrese částečně (případně také včetně StreetPartial a PremisesPartial).</span><span class="sxs-lookup"><span data-stu-id="261af-139">There are multiple fields that are partial in the address (potentially also including StreetPartial and PremisesPartial).</span></span> | <span data-ttu-id="261af-140">Více – maximálně tři</span><span class="sxs-lookup"><span data-stu-id="261af-140">Multiple—maximum of three</span></span> |
| <span data-ttu-id="261af-141">Žádné</span><span class="sxs-lookup"><span data-stu-id="261af-141">None</span></span> | <span data-ttu-id="261af-142">Adresa je nesprávná.</span><span class="sxs-lookup"><span data-stu-id="261af-142">Address is incorrect.</span></span> | <span data-ttu-id="261af-143">Žádné</span><span class="sxs-lookup"><span data-stu-id="261af-143">None</span></span> |
| <span data-ttu-id="261af-144">NotValidated</span><span class="sxs-lookup"><span data-stu-id="261af-144">NotValidated</span></span> | <span data-ttu-id="261af-145">Adresu nelze odeslat prostřednictvím procesu ověřování.</span><span class="sxs-lookup"><span data-stu-id="261af-145">Address was not able to be sent through the validation process.</span></span>  | <span data-ttu-id="261af-146">Žádné</span><span class="sxs-lookup"><span data-stu-id="261af-146">None</span></span> |

<span data-ttu-id="261af-147">Po odeslání adresy, která se má ověřit prostřednictvím rozhraní ValidateAddress API, se vrátí následující schéma odpovědi:</span><span class="sxs-lookup"><span data-stu-id="261af-147">Once an address has been submitted to be validated via the ValidateAddress API, the following response schema will be returned:</span></span>

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

<span data-ttu-id="261af-148">Podívejte se na tuto ukázkovou odpověď.</span><span class="sxs-lookup"><span data-stu-id="261af-148">Take a look at this sample response.</span></span> <span data-ttu-id="261af-149">Všimněte si, že pro nás odpověď vrátí další příponu se čtyřmi číslicemi, pokud pro PSČ zadáte jenom pět číslic.</span><span class="sxs-lookup"><span data-stu-id="261af-149">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

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

### <a name="next-steps"></a><span data-ttu-id="261af-150">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-150">Next steps</span></span>

- <span data-ttu-id="261af-151">Sdílejte své ID tenanta izolovaného prostoru s naším odborníkem na danou problematiku (MSP), Ali pískově, který se má zahrnout do testovacího letu, abyste mohli začít připravovat aktualizaci.</span><span class="sxs-lookup"><span data-stu-id="261af-151">Share your sandbox tenant ID with our subject matter expert (SME), Ali Khaki, to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="261af-152">Pokud používáte řešení v rámci ovládacího panelu (CPV), obraťte se na CPV.</span><span class="sxs-lookup"><span data-stu-id="261af-152">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="261af-153">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="261af-153">Questions?</span></span>

<span data-ttu-id="261af-154">Pokud máte nějaké dotazy nebo potřebujete podporu pro vaše operace s Microsoftem, obraťte se na svého partnera, který podporuje Yammer.</span><span class="sxs-lookup"><span data-stu-id="261af-154">If you have any questions or need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="261af-155">Nové prostředí v centru pro správu Exchange (EAC)</span><span class="sxs-lookup"><span data-stu-id="261af-155">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="261af-156">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-156">Categories</span></span>

- <span data-ttu-id="261af-157">Datum: 2021-03-29</span><span class="sxs-lookup"><span data-stu-id="261af-157">Date: 2021-03-29</span></span>
- <span data-ttu-id="261af-158">Možnosti</span><span class="sxs-lookup"><span data-stu-id="261af-158">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="261af-159">Souhrn</span><span class="sxs-lookup"><span data-stu-id="261af-159">Summary</span></span>

<span data-ttu-id="261af-160">Od 27. dubna 2021 se v centru pro správu Exchange (EAC) zavádí nové prostředí, které bude zlepšit každodenní efektivitu pro uživatele.</span><span class="sxs-lookup"><span data-stu-id="261af-160">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-161">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-161">Impacted audience</span></span>

<span data-ttu-id="261af-162">Delegovaní správci přistupující k Exchangi prostřednictvím partnerského centra</span><span class="sxs-lookup"><span data-stu-id="261af-162">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="261af-163">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-163">Details</span></span>

<span data-ttu-id="261af-164">Od 27. dubna 2021 budou partneři, kteří se přecházejí na Exchange prostřednictvím partnerského centra, přesměrováni na nový EAC.</span><span class="sxs-lookup"><span data-stu-id="261af-164">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="261af-165">Toto nové prostředí je teď k dispozici ve verzi Preview a správci můžou aktivovat toto prostředí výběrem přepínače v pravém horním rohu v klasickém poli EAC.</span><span class="sxs-lookup"><span data-stu-id="261af-165">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="261af-166">Můžou také přejít k novému poli EAC tím, že vyberou banner "vyzkoušet ho Now", který se zobrazí na všech stránkách.</span><span class="sxs-lookup"><span data-stu-id="261af-166">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="261af-167">Mezi výhody nového pole EAC patří:</span><span class="sxs-lookup"><span data-stu-id="261af-167">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="261af-168">Přidání přehledů, sestav a mechanismů výstrah pro řízení toku pošty – problémy související s.</span><span class="sxs-lookup"><span data-stu-id="261af-168">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="261af-169">Individuální řídicí panely pro zvýšení produktivity.</span><span class="sxs-lookup"><span data-stu-id="261af-169">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="261af-170">K usnadnění navigace v novém prostředí jsou k dispozici videa v části **školení & příručka** na novém prostředí EAC.</span><span class="sxs-lookup"><span data-stu-id="261af-170">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="261af-171">Tyto informace vám poskytnou přehled o tom, jak můžete nový portál nejlépe využít.</span><span class="sxs-lookup"><span data-stu-id="261af-171">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="261af-172">V rámci této změny nebudou klasické prostředí EAC zastaralé.</span><span class="sxs-lookup"><span data-stu-id="261af-172">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="261af-173">Před implementací jakékoli změny se bude předem informovat.</span><span class="sxs-lookup"><span data-stu-id="261af-173">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="261af-174">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-174">Next steps</span></span>

- <span data-ttu-id="261af-175">Projděte si [materiály k tomuto tématu](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), kde můžete zobrazit snímky obrazovky nového prostředí.</span><span class="sxs-lookup"><span data-stu-id="261af-175">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="261af-176">Tyto informace sdílejte s příslušnými zúčastněnými stranami ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="261af-176">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="261af-177">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="261af-177">Questions?</span></span>

<span data-ttu-id="261af-178">Jakékoli otázky týkající se těchto změn najdete v příslušných komunitách Yammeru.</span><span class="sxs-lookup"><span data-stu-id="261af-178">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="261af-179">Operace s Microsoftem: Úvod do kalendářního spuštění produktu</span><span class="sxs-lookup"><span data-stu-id="261af-179">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="261af-180">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-180">Categories</span></span>

- <span data-ttu-id="261af-181">Datum: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="261af-181">Date: 2021-03-25</span></span>
- <span data-ttu-id="261af-182">Nabídky | Moderní pracoviště</span><span class="sxs-lookup"><span data-stu-id="261af-182">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="261af-183">Souhrn</span><span class="sxs-lookup"><span data-stu-id="261af-183">Summary</span></span>

<span data-ttu-id="261af-184">V reakci na zpětnou vazbu od partnerů budou operace společnosti Microsoft zjednodušovat komunikaci při spuštění produktu.</span><span class="sxs-lookup"><span data-stu-id="261af-184">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-185">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-185">Impacted audience</span></span>

<span data-ttu-id="261af-186">Partneři poskytovatele Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="261af-186">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="261af-187">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-187">Details</span></span>

<span data-ttu-id="261af-188">Společnost Microsoft se zavazuje nepřetržitě zdokonalit partnerské prostředí.</span><span class="sxs-lookup"><span data-stu-id="261af-188">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="261af-189">Máme vám zpětnou vazbu od vás, že od Microsoftu jste obdrželi příliš mnoho komunikací, včetně duplicitních oznámení o spuštění produktu.</span><span class="sxs-lookup"><span data-stu-id="261af-189">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="261af-190">V reakci na vaši zpětnou vazbu společnost Microsoft zjednodušila možnosti připravenosti na spuštění produktů pro nové a stávající nabídky.</span><span class="sxs-lookup"><span data-stu-id="261af-190">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="261af-191">Teď vám nabízíme měsíční pohled na spuštění produktu, který je publikovaný v galerii prostředků připravenosti na operace.</span><span class="sxs-lookup"><span data-stu-id="261af-191">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="261af-192">Tento měsíční [Náhled spuštění produktu](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) nahradí konkrétní komunikaci na spuštění produktu v galerii prostředků připravenosti na operace a v oznámeních partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="261af-192">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="261af-193">K tomuto [kalendáři](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) můžete také přistupovat z [kolekcí komunit](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [zobrazení kalendáře](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)a [bulletinů CSP](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span><span class="sxs-lookup"><span data-stu-id="261af-193">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="261af-194">Když publikujete kalendář pro spuštění produktu měsíčně s oznámením v galerii prostředků připravenosti na provoz, pošleme vám oznámení.</span><span class="sxs-lookup"><span data-stu-id="261af-194">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="261af-195">Informace týkající se nové a stávající nabídky najdete pořád v protokolech pro náhled ceníku a v protokolech změn ceníku a také v blogu k produktům, licenčních průvodcích a na stránkách pro marketing produktů.</span><span class="sxs-lookup"><span data-stu-id="261af-195">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="261af-196">Tato změna se bude vztahovat na spuštění následujících produktů:</span><span class="sxs-lookup"><span data-stu-id="261af-196">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="261af-197">Místní aplikace Dynamics</span><span class="sxs-lookup"><span data-stu-id="261af-197">Dynamics on-premises</span></span>
- <span data-ttu-id="261af-198">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="261af-198">Microsoft 365</span></span>
- <span data-ttu-id="261af-199">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="261af-199">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="261af-200">Windows</span><span class="sxs-lookup"><span data-stu-id="261af-200">Windows</span></span>
- <span data-ttu-id="261af-201">Server</span><span class="sxs-lookup"><span data-stu-id="261af-201">Server</span></span>  
- <span data-ttu-id="261af-202">nástroje</span><span class="sxs-lookup"><span data-stu-id="261af-202">Tools</span></span>
- <span data-ttu-id="261af-203">Týmy a výpovědi</span><span class="sxs-lookup"><span data-stu-id="261af-203">Teams and Telco</span></span>

<span data-ttu-id="261af-204">Budeme dál posílat konkrétní oznámení ke spuštění produktu, které vyžaduje podrobnosti o připravenosti na operace.</span><span class="sxs-lookup"><span data-stu-id="261af-204">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="261af-205">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-205">Next steps</span></span>

<span data-ttu-id="261af-206">Projděte si materiály k tomuto tématu a sdílejte tyto informace s příslušnými zúčastněnými stranami ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="261af-206">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="261af-207">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="261af-207">Questions?</span></span>

<span data-ttu-id="261af-208">Další otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.</span><span class="sxs-lookup"><span data-stu-id="261af-208">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="261af-209">Změny požadavků na registraci zprostředkovatele CSP pro zákazníky</span><span class="sxs-lookup"><span data-stu-id="261af-209">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="261af-210">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-210">Categories</span></span>

- <span data-ttu-id="261af-211">Datum: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="261af-211">Date: 2021-03-25</span></span>
- <span data-ttu-id="261af-212">Možnosti</span><span class="sxs-lookup"><span data-stu-id="261af-212">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="261af-213">Souhrn</span><span class="sxs-lookup"><span data-stu-id="261af-213">Summary</span></span>

<span data-ttu-id="261af-214">V rámci našeho závazku pomáhat partnerům a zákazníkům, kteří provozují své podnikání na základě důvěry, budeme požadovat další informace o zákaznících, účinnost 25. března 2021.</span><span class="sxs-lookup"><span data-stu-id="261af-214">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-215">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-215">Impacted audience</span></span>

<span data-ttu-id="261af-216">Partneři poskytovatele Cloud Solution Provider (CSP) a nepřímá poskytovatelé, kteří mají nové nebo existující zákazníky v zemích uvedených v další části</span><span class="sxs-lookup"><span data-stu-id="261af-216">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="261af-217">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-217">Details</span></span>

<span data-ttu-id="261af-218">Microsoft běží na důvěryhodnosti.</span><span class="sxs-lookup"><span data-stu-id="261af-218">Microsoft runs on trust.</span></span> <span data-ttu-id="261af-219">Zavázali jsme se poskytovat vyhovující, bezpečné a zabezpečené metody ověřování zákazníků pro transakce předplatných zákazníka v programu CSP.</span><span class="sxs-lookup"><span data-stu-id="261af-219">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="261af-220">25. března 2021 budeme zavádět vylepšení rozhraní API partnerského centra a uživatelského rozhraní, které bude mít vliv na partnery, kteří splňují obě následující kritéria:</span><span class="sxs-lookup"><span data-stu-id="261af-220">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="261af-221">Partner má přímý fakturační vztah s Microsoftem (to znamená, že partner je buď přímým partnerem, nebo nepřímým poskytovatelem).</span><span class="sxs-lookup"><span data-stu-id="261af-221">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="261af-222">Partner pracuje s novými nebo stávajícími zákazníky v těchto zemích:</span><span class="sxs-lookup"><span data-stu-id="261af-222">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="261af-223">Thajsko</span><span class="sxs-lookup"><span data-stu-id="261af-223">Thailand</span></span>
    - <span data-ttu-id="261af-224">Vietnam</span><span class="sxs-lookup"><span data-stu-id="261af-224">Vietnam</span></span>
    - <span data-ttu-id="261af-225">Turecko</span><span class="sxs-lookup"><span data-stu-id="261af-225">Turkey</span></span>
    - <span data-ttu-id="261af-226">Polsko</span><span class="sxs-lookup"><span data-stu-id="261af-226">Poland</span></span>
    - <span data-ttu-id="261af-227">Jižní Afrika</span><span class="sxs-lookup"><span data-stu-id="261af-227">South Africa</span></span>
    - <span data-ttu-id="261af-228">Indie</span><span class="sxs-lookup"><span data-stu-id="261af-228">India</span></span>
    - <span data-ttu-id="261af-229">Brazílie</span><span class="sxs-lookup"><span data-stu-id="261af-229">Brazil</span></span>
    - <span data-ttu-id="261af-230">Irák</span><span class="sxs-lookup"><span data-stu-id="261af-230">Iraq</span></span>
    - <span data-ttu-id="261af-231">Myanmar</span><span class="sxs-lookup"><span data-stu-id="261af-231">Myanmar</span></span>
    - <span data-ttu-id="261af-232">Jižní Súdán</span><span class="sxs-lookup"><span data-stu-id="261af-232">South Sudan</span></span>
    - <span data-ttu-id="261af-233">Saúdská Arábie</span><span class="sxs-lookup"><span data-stu-id="261af-233">Saudi Arabia</span></span>
    - <span data-ttu-id="261af-234">Spojené arabské emiráty</span><span class="sxs-lookup"><span data-stu-id="261af-234">United Arab Emirates</span></span>
    - <span data-ttu-id="261af-235">Venezuela</span><span class="sxs-lookup"><span data-stu-id="261af-235">Venezuela</span></span>

<span data-ttu-id="261af-236">Partneři, kteří splňují kritéria, budou muset odeslat **registrační ID společnosti** zákazníka (označované také jako **DIČ organizace** zákazníka) a **telefonní číslo** , když připojí nové zákazníky nebo změní stávající podrobnosti o zákaznících.</span><span class="sxs-lookup"><span data-stu-id="261af-236">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="261af-237">Tito partneři můžou volitelně zadat také **druhé jméno** zákazníka.</span><span class="sxs-lookup"><span data-stu-id="261af-237">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="261af-238">Všimněte si, že při přidání registračního ID vaší společnosti byste měli použít své obchodní daňové ID, nikoli osobní ID zákazníka.</span><span class="sxs-lookup"><span data-stu-id="261af-238">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="261af-239">Partneři, kteří pracují s novými nebo stávajícími zákazníky v následujících zemích, už jsou připojení k předchozí verzi v listopadu 2020.</span><span class="sxs-lookup"><span data-stu-id="261af-239">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="261af-240">Arménie</span><span class="sxs-lookup"><span data-stu-id="261af-240">Armenia</span></span>
- <span data-ttu-id="261af-241">Ázerbájdžán</span><span class="sxs-lookup"><span data-stu-id="261af-241">Azerbaijan</span></span>
- <span data-ttu-id="261af-242">Bělorusko</span><span class="sxs-lookup"><span data-stu-id="261af-242">Belarus</span></span>
- <span data-ttu-id="261af-243">Maďarsko</span><span class="sxs-lookup"><span data-stu-id="261af-243">Hungary</span></span>
- <span data-ttu-id="261af-244">Kazachstán</span><span class="sxs-lookup"><span data-stu-id="261af-244">Kazakhstan</span></span>
- <span data-ttu-id="261af-245">Kyrgyzstán</span><span class="sxs-lookup"><span data-stu-id="261af-245">Kyrgyzstan</span></span>
- <span data-ttu-id="261af-246">Moldavsko</span><span class="sxs-lookup"><span data-stu-id="261af-246">Moldova</span></span>
- <span data-ttu-id="261af-247">Rusko</span><span class="sxs-lookup"><span data-stu-id="261af-247">Russia</span></span>
- <span data-ttu-id="261af-248">Tádžikistán</span><span class="sxs-lookup"><span data-stu-id="261af-248">Tajikistan</span></span>
- <span data-ttu-id="261af-249">Ukrajina</span><span class="sxs-lookup"><span data-stu-id="261af-249">Ukraine</span></span>
- <span data-ttu-id="261af-250">Uzbekistán</span><span class="sxs-lookup"><span data-stu-id="261af-250">Uzbekistan</span></span>

<span data-ttu-id="261af-251">Partneři se zákazníky ve zbývající části světa budou mít možnost 25. března 2021 pro zadání **ID registrace společnosti**, **telefonního čísla** a **středního jména** pro zákazníky jako volitelné podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="261af-251">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="261af-252">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-252">Next steps</span></span>

- <span data-ttu-id="261af-253">Podrobnější pokyny najdete v technické dokumentaci a nejčastější dotazy v [kolekci vyhrazených partnerů](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) .</span><span class="sxs-lookup"><span data-stu-id="261af-253">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="261af-254">Připravte se na začlenění změn pomocí rozhraní API partnerského centra a uživatelského prostředí pro web.</span><span class="sxs-lookup"><span data-stu-id="261af-254">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="261af-255">Pro testování bude k dispozici rozhraní API/sady SDK.</span><span class="sxs-lookup"><span data-stu-id="261af-255">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="261af-256">Nezapomeňte odeslat další data při připojování nových zákazníků nebo úpravách stávajících informací o zákaznících.</span><span class="sxs-lookup"><span data-stu-id="261af-256">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="261af-257">Pokud používáte řešení v rámci ovládacího panelu (CPV), obraťte se na CPV.</span><span class="sxs-lookup"><span data-stu-id="261af-257">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="261af-258">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="261af-258">Questions?</span></span>

<span data-ttu-id="261af-259">Pokud máte dotazy související s platným identifikátorem (označovaným také jako DIČ nebo DIČ), kontaktujte daňového poradce nebo místní finanční kancelář.</span><span class="sxs-lookup"><span data-stu-id="261af-259">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="261af-260">Microsoft nemůže poskytnout pokyny k daňovým aspektům.</span><span class="sxs-lookup"><span data-stu-id="261af-260">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="261af-261">Pokud potřebujete podporu v rámci svých operací s Microsoftem, [otevřete žádost o služby](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="261af-261">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="261af-262">Opravy provedené 1. března 2021, což je trvalá Ceníková cena softwaru</span><span class="sxs-lookup"><span data-stu-id="261af-262">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="261af-263">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-263">Categories</span></span>

- <span data-ttu-id="261af-264">Datum: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="261af-264">Date: 2021-03-23</span></span>
- <span data-ttu-id="261af-265">Nabídky/trhy</span><span class="sxs-lookup"><span data-stu-id="261af-265">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-266">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-266">Impacted audience</span></span>

<span data-ttu-id="261af-267">Nepřímá poskytovatelé a Přímí partneři poskytující transakční transakce s probíhajícím softwarem v programu Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="261af-267">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="261af-268">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-268">Details</span></span>

<span data-ttu-id="261af-269">Ceník pro trvale zpracovaný software zveřejněný 1. března 2021 zahrnoval trhy, které by se tam nemusely nastavovat.</span><span class="sxs-lookup"><span data-stu-id="261af-269">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="261af-270">Ceník trvalého softwaru byl aktualizován 17. března 2021 se opravami.</span><span class="sxs-lookup"><span data-stu-id="261af-270">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="261af-271">Tyto opravy byly platné pouze pro:</span><span class="sxs-lookup"><span data-stu-id="261af-271">These corrections were only applicable to:</span></span>

- <span data-ttu-id="261af-272">ID produktu: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="261af-272">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="261af-273">Název produktu: upgrade Windows 10 Home na verzi pro pro Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="261af-273">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="261af-274">Odebrané nebo nepodporované trhy: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, ČERNOBÍLé, by, BZ, CI, CL, CM, CO, CR, SH, DO, DZ, ES, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, SWEETIQ, JM, JO, KE, KG, KN, KW, KY, KZ, CR, LK, LY, MA, MC, MD, já, MN, M0, , NI,, NP, OM, PA, PE, PH, PK, PR, PY, QA, R, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, G, UY, UZ, VE, VN, BE, ZM, ZW</span><span class="sxs-lookup"><span data-stu-id="261af-274">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="261af-275">Tyto změny se vztahují pouze na výše uvedený produkt.</span><span class="sxs-lookup"><span data-stu-id="261af-275">These changes only apply to the above product.</span></span> <span data-ttu-id="261af-276">Jiné produkty neobsahovaly žádné opravy.</span><span class="sxs-lookup"><span data-stu-id="261af-276">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="261af-277">Další kroky a zdroje informací</span><span class="sxs-lookup"><span data-stu-id="261af-277">Next steps and resources</span></span>

- <span data-ttu-id="261af-278">Partneři, kteří pracují s nezpracovaným softwarem, by si měli stáhnout nejnovější Ceník softwaru s trvalou cenou.</span><span class="sxs-lookup"><span data-stu-id="261af-278">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="261af-279">V části [kódy zemí v oblasti](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) najdete popisné mapování obou zkratek na země.</span><span class="sxs-lookup"><span data-stu-id="261af-279">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> <span data-ttu-id="261af-280">Vydání sady SDK na .NET Standard (v 1.17.0)</span><span class="sxs-lookup"><span data-stu-id="261af-280">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="261af-281">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-281">Categories</span></span>

- <span data-ttu-id="261af-282">Datum: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="261af-282">Date: 2021-03-23</span></span>

- <span data-ttu-id="261af-283">Možnosti</span><span class="sxs-lookup"><span data-stu-id="261af-283">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="261af-284">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-284">Impacted audience</span></span>

<span data-ttu-id="261af-285">Přímé partnery a nepřímá poskytovatelé, kteří se účastní programu CSP, kteří používají sadu SDK pro partnerských Center.</span><span class="sxs-lookup"><span data-stu-id="261af-285">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="261af-286">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-286">Details</span></span>

<span data-ttu-id="261af-287">Od března 23 2020 můžou partneři začít stahovat verzi [MicrosoftPartnerCenter. NETSDK (galerie NuGet | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)spolu s aktualizovanými [ukázkami](https://github.com/Microsoft/Partner-Center-DotNet-Samples)služby Public partner Center SDK GitHub.</span><span class="sxs-lookup"><span data-stu-id="261af-287">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="261af-288">Tato verze zahrnuje aktualizace následujících metod:</span><span class="sxs-lookup"><span data-stu-id="261af-288">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="261af-289">Audit byl aktualizován: nové typy operací</span><span class="sxs-lookup"><span data-stu-id="261af-289">Audit Updated: New operation types</span></span>

<span data-ttu-id="261af-290">Přidání nových [typů operací](https://docs.microsoft.com/partner-center/develop/auditing-resources) pro znalost, kdy zákazník schválil a ukončil DAP.</span><span class="sxs-lookup"><span data-stu-id="261af-290">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="261af-291">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="261af-291">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="261af-292">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="261af-292">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="261af-293">Audit byl aktualizován: nové typy prostředků a operací</span><span class="sxs-lookup"><span data-stu-id="261af-293">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="261af-294">Přidali jsme nové [typy prostředků a operací](https://docs.microsoft.com/partner-center/develop/auditing-resources) pro podporu scénáře role adresáře zákazníka.</span><span class="sxs-lookup"><span data-stu-id="261af-294">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="261af-295">Nový typ prostředku "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="261af-295">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="261af-296">Typy operací "AddUserMember" a "RemoveUserMember"</span><span class="sxs-lookup"><span data-stu-id="261af-296">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="261af-297">Aktualizace sady SDK u zákaznických účtů</span><span class="sxs-lookup"><span data-stu-id="261af-297">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="261af-298">Podpora pro GET/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span><span class="sxs-lookup"><span data-stu-id="261af-298">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="261af-299">ZÍSKAT/Customers/{Customer-tenant-ID}/Qualifications</span><span class="sxs-lookup"><span data-stu-id="261af-299">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="261af-300">POST/Customers/{customer_id}/Qualifications? Code = {validationCode}</span><span class="sxs-lookup"><span data-stu-id="261af-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="261af-301">Další změny</span><span class="sxs-lookup"><span data-stu-id="261af-301">Additional changes</span></span>

<span data-ttu-id="261af-302">V rámci nového obchodu byly zavedeny následující změny, které jsou aktuálně k dispozici pouze partnerům, kteří jsou součástí M365/D365 New Commerce Experience Technical Preview.</span><span class="sxs-lookup"><span data-stu-id="261af-302">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="261af-303">Partneři, kteří nejsou součástí nové verze nástroje Commerce Technical Preview, by neměli poznamenat dopady a měly by být zpětně kompatibilní.</span><span class="sxs-lookup"><span data-stu-id="261af-303">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="261af-304">Změny katalogu:</span><span class="sxs-lookup"><span data-stu-id="261af-304">Catalog Changes:</span></span>

  - <span data-ttu-id="261af-305">ZÍSKAT/Products/{Product-ID}/skus/{SKU-ID}</span><span class="sxs-lookup"><span data-stu-id="261af-305">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="261af-306">Nákup a správa:</span><span class="sxs-lookup"><span data-stu-id="261af-306">Purchase and Manage:</span></span>
  - <span data-ttu-id="261af-307">ZÍSKAT/customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="261af-307">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="261af-308">ZÍSKAT/customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="261af-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="261af-309">/Customers/{customerId}/subscriptions/{subscriptionId} opravy</span><span class="sxs-lookup"><span data-stu-id="261af-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="261af-310">ZÍSKAT/customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="261af-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="261af-311">ZÍSKAT/customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="261af-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="261af-312">PŘÍSPĚVEK/customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="261af-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="261af-313">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-313">Next Steps</span></span>

- <span data-ttu-id="261af-314">Stáhněte si nejnovější verzi [MicrosoftPartnerCenter. NETSDK (galerie NuGet | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span><span class="sxs-lookup"><span data-stu-id="261af-314">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="261af-315">Stažení a kontrola [ukázek GitHubu](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span><span class="sxs-lookup"><span data-stu-id="261af-315">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="261af-316">Nabídka CSP pro komerční web Marketplace a FY21 CSP pro opravňující nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-316">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="261af-317">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-317">Categories</span></span>

- <span data-ttu-id="261af-318">Datum: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="261af-318">Date: 2021-03-18</span></span>
- <span data-ttu-id="261af-319">Možnosti</span><span class="sxs-lookup"><span data-stu-id="261af-319">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-320">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-320">Impacted audience</span></span>

<span data-ttu-id="261af-321">Neposkytovatelé nepřímých zprostředkovatelů a přímých partnerů v programu Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="261af-321">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="261af-322">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-322">Details</span></span>

<span data-ttu-id="261af-323">Nepřímá poskytovatelé a přímá Partnerská partneři v programu Cloud Solution Provider můžou prodávat nabídky třetích stran a získat motivaci slev pro každou způsobilou nabídku třetí strany, která je v partnerském centru nebo Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="261af-323">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="261af-324">Motivace bude ve formě rabatu na účtovaných prodejích pro příslušné nabídky a bude **k dispozici do 30. června 2021**.</span><span class="sxs-lookup"><span data-stu-id="261af-324">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="261af-325">Pokračujte v učení o této nabídce komerčního webu Web Marketplace níže a kontaktujte své zákazníky ještě dnes a Identifikujte správné nabídky, které umožní jejich pokračující úspěšnost a digitální transformaci.</span><span class="sxs-lookup"><span data-stu-id="261af-325">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="261af-326">Spolupracujeme s nezávislými výrobci softwaru (ISV) za účelem uvedení nejnovějších řešení IaaS a SaaS na trh pro zákazníky Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="261af-326">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="261af-327">Vydavatelé ISV mají možnost povolit prodej svých nabídek prostřednictvím kanálu Microsoft Partner.</span><span class="sxs-lookup"><span data-stu-id="261af-327">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="261af-328">Naše pobídkové nabídky spadají do dvou kategorií:</span><span class="sxs-lookup"><span data-stu-id="261af-328">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="261af-329">Vyberte SaaS a IaaS nabídky třetích stran pomocí Azure IP spoluprodejního stavu motivovaní.</span><span class="sxs-lookup"><span data-stu-id="261af-329">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="261af-330">SaaS aplikace integrované s týmy nebo aspoň dvě Microsoft 365 kancelářské aplikace, jako je PowerPoint, Word, Excel, Outlook nebo SharePoint.</span><span class="sxs-lookup"><span data-stu-id="261af-330">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="261af-331">Další kroky a zdroje informací</span><span class="sxs-lookup"><span data-stu-id="261af-331">Next steps and resources</span></span>

- <span data-ttu-id="261af-332">Přečtěte si, jak získat [pobídky partnerských](https://partner.microsoft.com/membership/partner-incentives) webů pro prodej oprávněných aplikací na webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="261af-332">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="261af-333">Nové nabídky se přidávají měsíčně.</span><span class="sxs-lookup"><span data-stu-id="261af-333">New offers are added monthly.</span></span>  
- [<span data-ttu-id="261af-334">Prostředky pro definanční partnery poskytovatele Cloud Solution Provider Direct</span><span class="sxs-lookup"><span data-stu-id="261af-334">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="261af-335">Prostředky pro motivaci nepřímých poskytovatelů Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="261af-335">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="261af-336">Přečtěte si tuto [prezentaci](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) , kde najdete další informace o prodeji komerčních aplikací z webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="261af-336">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="261af-337">Další materiály najdete [tady](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span><span class="sxs-lookup"><span data-stu-id="261af-337">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="261af-338">Prozkoumejte katalog komerčního tržiště v [partnerském centru](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) nebo [Azure Portal](https://ms.portal.azure.com/#home)</span><span class="sxs-lookup"><span data-stu-id="261af-338">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="261af-339">Použití [rozhraní API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) k integraci aplikací do Marketplace vaší společnosti</span><span class="sxs-lookup"><span data-stu-id="261af-339">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="261af-340">Přihlaste se k nezávislým výrobcům softwaru, se kterým se zajímá vaše podnikání</span><span class="sxs-lookup"><span data-stu-id="261af-340">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="261af-341">Neposkytovatelé nepřímých zprostředkovatelů potřebují integrovat pomocí rozhraní API a prodejců s postupy, na kterých se aplikace prodávají.</span><span class="sxs-lookup"><span data-stu-id="261af-341">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="261af-342">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="261af-342">Questions?</span></span>  

<span data-ttu-id="261af-343">V [tomto článku](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) najdete přehled komerčního tržiště v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="261af-343">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="261af-344">Pokud potřebujete další pomoc, můžete vytvořit žádost o podporu v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="261af-344">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="261af-345">Další informace najdete na adrese [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="261af-345">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="261af-346">Power BI Premium nabídky pro pojmenování a požadované aktualizace</span><span class="sxs-lookup"><span data-stu-id="261af-346">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="261af-347">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-347">Categories</span></span>

- <span data-ttu-id="261af-348">Datum: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="261af-348">Date: 2021-03-18</span></span>
- <span data-ttu-id="261af-349">Možnosti</span><span class="sxs-lookup"><span data-stu-id="261af-349">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="261af-350">Souhrn</span><span class="sxs-lookup"><span data-stu-id="261af-350">Summary</span></span>

<span data-ttu-id="261af-351">Konečný Ceník od 1. dubna 2021 se aktualizuje, aby se zvýšila přesnost na pojmenování a informace o požadavcích pro Power BI Premium pro jednotlivé uživatele.</span><span class="sxs-lookup"><span data-stu-id="261af-351">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-352">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-352">Impacted audience</span></span>

<span data-ttu-id="261af-353">Přímý a nepřímý partneři poskytovatele Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="261af-353">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="261af-354">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-354">Details</span></span>

<span data-ttu-id="261af-355">Konečný Ceník od 1. dubna 2021 se aktualizuje, aby se zvýšila přesnost na pojmenování a informace o požadavcích pro Power BI Premium pro jednotlivé uživatele.</span><span class="sxs-lookup"><span data-stu-id="261af-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="261af-356">Až do doby, kdy se aktualizuje Poslední ceník, použijte informace v této části, abyste zajistili, že se správně objednal správný produkt.</span><span class="sxs-lookup"><span data-stu-id="261af-356">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="261af-357">Následující podrobnosti obsahují informace o ovlivněné SKU a požadovaných položkách.</span><span class="sxs-lookup"><span data-stu-id="261af-357">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="261af-358">Zobrazované jméno nabídky na 1. březnu Preview ceníku</span><span class="sxs-lookup"><span data-stu-id="261af-358">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="261af-359">Aktualizovaný zobrazovaný název nabídky na 1. dubnu – konečný Ceník</span><span class="sxs-lookup"><span data-stu-id="261af-359">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="261af-360">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-360">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="261af-361">Power BI Premium Add-On na uživatele (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="261af-361">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="261af-362">Power BI Premium pro uživatele Add-On **(Office)** (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="261af-362">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="261af-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="261af-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="261af-364">Aby si zákazníci mohli koupit tuto nabídku, musí mít některý z následujících požadavků:</span><span class="sxs-lookup"><span data-stu-id="261af-364">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="261af-365">Zobrazované jméno nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-365">Offer display name</span></span> | <span data-ttu-id="261af-366">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-366">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="261af-367">Microsoft 365 E5 (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="261af-367">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="261af-368">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="261af-368">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="261af-369">Microsoft 365 E5 bez audio Conferencing (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="261af-369">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="261af-370">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="261af-370">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="261af-371">Office 365 E5 (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="261af-371">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="261af-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="261af-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="261af-373">Zkušební verze Office 365 E5 (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="261af-373">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="261af-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="261af-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="261af-375">Office 365 E5 bez audio Conferencing (ceny za neziskové zaměstnance)</span><span class="sxs-lookup"><span data-stu-id="261af-375">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="261af-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="261af-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="261af-377">Pro nákup je nutné mít následující nabídku Power BI Premium:</span><span class="sxs-lookup"><span data-stu-id="261af-377">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="261af-378">Zobrazované jméno nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-378">Offer display name</span></span> | <span data-ttu-id="261af-379">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-379">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="261af-380">Power BI Premium Add-On na uživatele (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="261af-380">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="261af-381">ef0b895b-681B-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="261af-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="261af-382">Aby si zákazníci mohli koupit tuto nabídku, musí mít tyto předpoklady:</span><span class="sxs-lookup"><span data-stu-id="261af-382">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="261af-383">Zobrazované jméno nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-383">Offer display name</span></span> | <span data-ttu-id="261af-384">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-384">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="261af-385">Power BI Pro (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="261af-385">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="261af-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="261af-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="261af-387">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-387">Next steps</span></span>

<span data-ttu-id="261af-388">Projděte si materiály k tomuto tématu a sdílejte tyto informace s příslušnými zúčastněnými stranami ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="261af-388">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="261af-389">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="261af-389">Questions?</span></span>

<span data-ttu-id="261af-390">Jakékoli otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.</span><span class="sxs-lookup"><span data-stu-id="261af-390">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> <span data-ttu-id="261af-391">Aktualizace ceny pro Microsoft 365 F3 v březnu</span><span class="sxs-lookup"><span data-stu-id="261af-391">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="261af-392">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-392">Categories</span></span>

- <span data-ttu-id="261af-393">Datum: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="261af-393">Date: 2021-03-16</span></span>
- <span data-ttu-id="261af-394">Nabídky/trhy</span><span class="sxs-lookup"><span data-stu-id="261af-394">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="261af-395">Souhrn</span><span class="sxs-lookup"><span data-stu-id="261af-395">Summary</span></span>

<span data-ttu-id="261af-396">Nesprávná cena z března 2021 byla opravena pro Microsoft 365 F3, British (GBP) a eura (EUR).</span><span class="sxs-lookup"><span data-stu-id="261af-396">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-397">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-397">Impacted audience</span></span>

<span data-ttu-id="261af-398">Partneři kupují Microsoft 365 F3 v GBP nebo EUR v rozmezí od 1. března 2021 v rámci programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="261af-398">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="261af-399">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-399">Details</span></span>

<span data-ttu-id="261af-400">Společnost Microsoft vyřešila nesprávné ceny za Microsoft 365 F3.</span><span class="sxs-lookup"><span data-stu-id="261af-400">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="261af-401">Nesprávné ceny jsou pro GBP a EUR a jenom pro nabídky zakoupené v rozmezí od 1. března 2021.</span><span class="sxs-lookup"><span data-stu-id="261af-401">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="261af-402">Ovlivněné nabídky a měny jsou uvedeny níže.</span><span class="sxs-lookup"><span data-stu-id="261af-402">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="261af-403">Název nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-403">Offer name</span></span> | <span data-ttu-id="261af-404">Měna</span><span class="sxs-lookup"><span data-stu-id="261af-404">Currency</span></span> | <span data-ttu-id="261af-405">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-405">Offer ID</span></span> | <span data-ttu-id="261af-406">ID materiálu</span><span class="sxs-lookup"><span data-stu-id="261af-406">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="261af-407">Microsoft 365 F3 (dobročinný)</span><span class="sxs-lookup"><span data-stu-id="261af-407">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="261af-408">GBP</span><span class="sxs-lookup"><span data-stu-id="261af-408">GBP</span></span> | <span data-ttu-id="261af-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="261af-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="261af-410">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="261af-410">AAD-11626</span></span> |
| <span data-ttu-id="261af-411">Microsoft 365 F3 (komerční)</span><span class="sxs-lookup"><span data-stu-id="261af-411">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="261af-412">EUR</span><span class="sxs-lookup"><span data-stu-id="261af-412">EUR</span></span>| <span data-ttu-id="261af-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="261af-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="261af-414">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="261af-414">AAA-89898</span></span> |
 
<span data-ttu-id="261af-415">Licence na březen a duben Preview – základní ceníky byly aktualizovány 16. března 17:00 tichomořského času (běžný čas).</span><span class="sxs-lookup"><span data-stu-id="261af-415">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="261af-416">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-416">Next steps</span></span>

- <span data-ttu-id="261af-417">Partneři by si měli stáhnout aktuální ceníky založené na licencích, a to v březnu i v dubnu Preview. Tyto ceny se v případě potřeby opraví.</span><span class="sxs-lookup"><span data-stu-id="261af-417">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="261af-418">Společnost Microsoft bude kontaktovat dotčené partnery v nadcházejících týdnech prostřednictvím e-mailu, aby jim informovala o dalších krocích souvisejících s opravou ovlivněných transakcí.</span><span class="sxs-lookup"><span data-stu-id="261af-418">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="261af-419">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="261af-419">Questions?</span></span>

<span data-ttu-id="261af-420">Jakékoli další otázky vám poskytne příslušné komunity zprostředkovatele CSP pro Yammer.</span><span class="sxs-lookup"><span data-stu-id="261af-420">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="261af-421">Aktualizace názvu právní společnosti prostřednictvím partnerského centra</span><span class="sxs-lookup"><span data-stu-id="261af-421">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="261af-422">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-422">Categories</span></span>

- <span data-ttu-id="261af-423">Datum: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="261af-423">Date: 2021-03-16</span></span>
- <span data-ttu-id="261af-424">Škálování & škály při zvyšování produktivity</span><span class="sxs-lookup"><span data-stu-id="261af-424">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="261af-425">Souhrn</span><span class="sxs-lookup"><span data-stu-id="261af-425">Summary</span></span>

<span data-ttu-id="261af-426">Od března 2021 se partneři Microsoft Partner Network (MPN) a poskytovatelé Cloud Solution Provider (CSP) můžou prostřednictvím partnerského centra aktualizovat svůj zákonný název společnosti.</span><span class="sxs-lookup"><span data-stu-id="261af-426">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-427">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-427">Impacted audience</span></span>

<span data-ttu-id="261af-428">Partneři programu MPN a neposkytovatelé nepřímých poskytovatelů CSP (neplatí pro partnery s přímým účtováním CSP)</span><span class="sxs-lookup"><span data-stu-id="261af-428">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="261af-429">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-429">Details</span></span>

<span data-ttu-id="261af-430">Od března 2021 partneři programu MPN a nepřímý prodej CSP můžou aktualizovat svůj právní název společnosti prostřednictvím partnerského centra v souladu se svým vlastním způsobem.</span><span class="sxs-lookup"><span data-stu-id="261af-430">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="261af-431">S touto novou funkcí už partneři nebudou muset odeslat lístek podpory pro partnerský partner, aby aktualizovali jeho název společnosti.</span><span class="sxs-lookup"><span data-stu-id="261af-431">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="261af-432">Tím se při provádění těchto aktivit uloží značná doba pro partnery.</span><span class="sxs-lookup"><span data-stu-id="261af-432">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="261af-433">Další informace najdete v tématu [aktualizace svého obchodního profilu](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="261af-433">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="261af-434">Ujistěte se, že název společnosti ve vašem oficiálním obchodním profilu není bez pravopisných chyb a zkratek a přesně odpovídá vašim oficiálním registračním záznamům společnosti.</span><span class="sxs-lookup"><span data-stu-id="261af-434">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="261af-435">Další informace o aktualizaci profilu vaší organizace najdete v tématu [ověření profilu vaší organizace](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="261af-435">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="261af-436">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-436">Next steps</span></span>

<span data-ttu-id="261af-437">Tyto informace můžete sdílet v rámci organizace, aby mohl příslušný tým zkontrolovat a aktualizovat své procesy.</span><span class="sxs-lookup"><span data-stu-id="261af-437">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="261af-438">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="261af-438">Questions?</span></span>

<span data-ttu-id="261af-439">Jakékoli další otázky vám poskytne příslušné komunity zprostředkovatele CSP pro Yammer.</span><span class="sxs-lookup"><span data-stu-id="261af-439">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="261af-440">Aktualizace pro vývoj programu Cloud Solution Provider (CSP) a Open License změny programu</span><span class="sxs-lookup"><span data-stu-id="261af-440">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="261af-441">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-441">Categories</span></span>

- <span data-ttu-id="261af-442">Datum: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="261af-442">Date: 2021-03-15</span></span>
- <span data-ttu-id="261af-443">Možnosti</span><span class="sxs-lookup"><span data-stu-id="261af-443">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="261af-444">Souhrn</span><span class="sxs-lookup"><span data-stu-id="261af-444">Summary</span></span>

<span data-ttu-id="261af-445">Nový komerční a veřejný sektor trvalé nabídky softwaru přicházejí do programu Cloud Solution Provider (CSP) spolu se změnami v programu Open Licensing.</span><span class="sxs-lookup"><span data-stu-id="261af-445">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-446">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-446">Impacted audience</span></span>

<span data-ttu-id="261af-447">Komerční distributoři a spravováni prodejci se prodávají prostřednictvím Open License programu a také všichni partneři CSP s podporou trvalého softwaru.</span><span class="sxs-lookup"><span data-stu-id="261af-447">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="261af-448">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-448">Details</span></span>

<span data-ttu-id="261af-449">V září 2020 společnost Microsoft [oznámila](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) řadu kroků v naší cestě k digitální transformaci, aby bylo možné rozšiřovat příležitosti pro partnery v programu CSP, včetně dostupnosti místního softwaru pro partnery.</span><span class="sxs-lookup"><span data-stu-id="261af-449">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="261af-450">Tyto změny umožňují partnerům rozšiřovat svou firmu a rozšířit jejich dosah tím, že využívají licence na software v cloudu, a jejich umístění pro úspěch v dnešním cloudovém světě.</span><span class="sxs-lookup"><span data-stu-id="261af-450">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="261af-451">Umožňují také přechody zákazníků do cloudu a poskytují partnerům potřebnou flexibilitu pro hybridní cloudová prostředí zákazníka.</span><span class="sxs-lookup"><span data-stu-id="261af-451">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="261af-452">V návaznosti na tuto digitální transformaci oznamujeme následující změny:</span><span class="sxs-lookup"><span data-stu-id="261af-452">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="261af-453">1. července 2021: do ceníku Open License programu nebudou přidány žádné nové SKU, produkty ani propagační akce.</span><span class="sxs-lookup"><span data-stu-id="261af-453">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="261af-454">7. července 2021: dvě komerční nabídky, Získejte originální Windows a Visual Studio Professional a nabídky veřejného sektoru (státní, vzdělávací a neziskové – viz [oznámení](./2020-december.md#9)) se přidají do ceníku trvalého softwaru CSP.</span><span class="sxs-lookup"><span data-stu-id="261af-454">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="261af-455">Ceník najdete v části software [nabídky prodej > price & nabízí](https://partnercenter.microsoft.com/pcv/sales) stránku v partnerském centru a bude se v tomto datu znovu publikovat.</span><span class="sxs-lookup"><span data-stu-id="261af-455">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="261af-456">Úplné podrobnosti týkající se vývoje programu CSP a Open License programových změn naleznete v **následujících krocích** níže.</span><span class="sxs-lookup"><span data-stu-id="261af-456">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="261af-457">Další kroky:</span><span class="sxs-lookup"><span data-stu-id="261af-457">Next Steps:</span></span>

- <span data-ttu-id="261af-458">Vývoj programu CSP: Projděte si [Trvalá softwarová řešení v materiálech připravenosti programu Cloud Solution Provider](https://partner.microsoft.com/resources/collection/software-in-csp#/) .</span><span class="sxs-lookup"><span data-stu-id="261af-458">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="261af-459">Pomocí této [mapy připravenosti](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) můžete rychle najít správné informace pro vaši roli.</span><span class="sxs-lookup"><span data-stu-id="261af-459">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="261af-460">Změny Open License programu: Přečtěte si materiály pro [vývoj programu CSP a Open License program změny](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) připravenosti.</span><span class="sxs-lookup"><span data-stu-id="261af-460">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="261af-461">Pomocí této [mapy připravenosti](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) můžete rychle najít správné informace pro vaši roli.</span><span class="sxs-lookup"><span data-stu-id="261af-461">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="261af-462">Dotazy</span><span class="sxs-lookup"><span data-stu-id="261af-462">Questions</span></span>

<span data-ttu-id="261af-463">Jakékoli další otázky vám poskytne příslušné komunity zprostředkovatele CSP pro Yammer.</span><span class="sxs-lookup"><span data-stu-id="261af-463">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="261af-464">Aktualizace na předchozí oznámení: posouzení Premium, doplněk ke Správci dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="261af-464">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="261af-465">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-465">Categories</span></span>

- <span data-ttu-id="261af-466">Datum: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="261af-466">Date: 2021-03-15</span></span>
- <span data-ttu-id="261af-467">Podpora růstu vaší firmy</span><span class="sxs-lookup"><span data-stu-id="261af-467">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="261af-468">Souhrn</span><span class="sxs-lookup"><span data-stu-id="261af-468">Summary</span></span>

<span data-ttu-id="261af-469">Nabídky zkušební verze by neměly být uvedené na ceníku a budou se odeberou.</span><span class="sxs-lookup"><span data-stu-id="261af-469">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-470">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-470">Impacted audience</span></span>

<span data-ttu-id="261af-471">Transakce partnerů prostřednictvím poskytovatele Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="261af-471">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="261af-472">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-472">Details</span></span>

<span data-ttu-id="261af-473">Ceník by neměl být zahrnut do ceníku.</span><span class="sxs-lookup"><span data-stu-id="261af-473">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="261af-474">Ty se odeberou z ceníku 1. května 2021.</span><span class="sxs-lookup"><span data-stu-id="261af-474">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="261af-475">Původní oznámení [najdete tady](./2021-february.md#4).</span><span class="sxs-lookup"><span data-stu-id="261af-475">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="261af-476">Další zdroje informací</span><span class="sxs-lookup"><span data-stu-id="261af-476">Additional resources</span></span>

- [<span data-ttu-id="261af-477">Microsoft 365 zabezpečení E5 a dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="261af-477">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="261af-478">Sestavování a Správa hodnocení v nástroji Microsoft dodržování předpisů – Microsoft 365 dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="261af-478">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="261af-479">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-479">Next steps</span></span>

<span data-ttu-id="261af-480">Projděte si materiály k tomuto tématu a sdílejte tyto informace s příslušnými zúčastněnými stranami ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="261af-480">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="261af-481">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="261af-481">Questions?</span></span>

<span data-ttu-id="261af-482">Otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.</span><span class="sxs-lookup"><span data-stu-id="261af-482">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="261af-483">Migrace řešení od jednoho komerčního partnera (OCP) přejít na trh (GTM) do komerčního tržiště Microsoftu</span><span class="sxs-lookup"><span data-stu-id="261af-483">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="261af-484">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-484">Categories</span></span>

- <span data-ttu-id="261af-485">Datum: 2021-03-12</span><span class="sxs-lookup"><span data-stu-id="261af-485">Date: 2021-03-12</span></span>
- <span data-ttu-id="261af-486">Možnosti</span><span class="sxs-lookup"><span data-stu-id="261af-486">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="261af-487">Souhrn</span><span class="sxs-lookup"><span data-stu-id="261af-487">Summary</span></span>

<span data-ttu-id="261af-488">Od 29. března 2021 zahájíte práci s omezeným počtem funkcí GTM (komerční partner), které se vztahují k uvedení na trh (OCP).</span><span class="sxs-lookup"><span data-stu-id="261af-488">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="261af-489">Doporučujeme migrovat vaše řešení na komerční tržiště v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="261af-489">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-490">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-490">Impacted audience</span></span>

<span data-ttu-id="261af-491">Organizace, které společně prodávají s řešeními v OCP GTM</span><span class="sxs-lookup"><span data-stu-id="261af-491">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="261af-492">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-492">Details</span></span>

<span data-ttu-id="261af-493">V prosinci 2020 jsme začali cestu od nástroje Microsoft OCP GTM k komerčnímu tržišti Microsoftu v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="261af-493">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="261af-494">Tento přechod rozšiřuje možnosti komerčního tržiště, kde můžete předprezentovat vaše řešení miliony zákazníků, obousměrně sdílet příležitosti s ostatními prodejci Microsoftu a partnerů a společně prodávat inovativní řešení.</span><span class="sxs-lookup"><span data-stu-id="261af-494">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="261af-495">Další milník v přechodu bude uskutečněn 29. března 2021.</span><span class="sxs-lookup"><span data-stu-id="261af-495">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="261af-496">To je, když začnete používat omezené možnosti OCP GTM, přičemž některá pole se stanou jen pro čtení.</span><span class="sxs-lookup"><span data-stu-id="261af-496">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="261af-497">Pokud v současné době spolupracujete s řešeními v OCP GTM, doporučujeme vám migrovat vaše řešení na komerční tržiště, abyste mohli využívat své možnosti a zjednodušili své možnosti publikování.</span><span class="sxs-lookup"><span data-stu-id="261af-497">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="261af-498">Přechod na komerční tržiště poskytuje partnerskému centru primární cíl pro spoluprodejní prostředí pro publikování.</span><span class="sxs-lookup"><span data-stu-id="261af-498">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="261af-499">Je to místo, kde můžete dál rozšiřovat své podnikání propojením vašich řešení s našimi sdílenými zákazníky přes stejné kanály a prostředí v produktu, které používáme pro produkty Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="261af-499">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="261af-500">[Přečtěte si další informace o komerčním tržišti](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span><span class="sxs-lookup"><span data-stu-id="261af-500">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="261af-501">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-501">Next steps</span></span>

- <span data-ttu-id="261af-502">Pokud jste vaše řešení ještě nepřesunuli, postupujte podle pokynů v [Průvodci přechodem](/azure/marketplace/co-sell-solution-migration) nebo si prohlédněte [podrobné výukové video](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) , které vám umožní dokončit všechny migrační aktivity a zahájit publikování vašich řešení na komerčním webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="261af-502">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="261af-503">Otázky týkající se omezeného prostředí funkcí v systému OCP GTM najdete v tématu [Nejčastější dotazy k požadavkům pro publikování na komerčním webu Microsoft Marketplace](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span><span class="sxs-lookup"><span data-stu-id="261af-503">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="261af-504">(Další informace najdete v části "OCP GTM – omezené možnosti od 29. března 2021.")</span><span class="sxs-lookup"><span data-stu-id="261af-504">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="261af-505">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="261af-505">Questions?</span></span>

<span data-ttu-id="261af-506">Pokud máte nějaké dotazy nebo potřebujete další informace, obraťte se na [podporu](https://partner.microsoft.com/support/?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="261af-506">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="261af-507">Rozšiřování nového prostředí pro obchod v programu Cloud Solution Provider (CSP) pro Azure na Rusko</span><span class="sxs-lookup"><span data-stu-id="261af-507">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="261af-508">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-508">Categories</span></span>

- <span data-ttu-id="261af-509">Datum: 2021-03-10</span><span class="sxs-lookup"><span data-stu-id="261af-509">Date: 2021-03-10</span></span>
- <span data-ttu-id="261af-510">Možnosti</span><span class="sxs-lookup"><span data-stu-id="261af-510">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-511">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-511">Impacted audience</span></span>

<span data-ttu-id="261af-512">Všichni partneři v Rusku procházejí v rámci programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="261af-512">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="261af-513">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-513">Details</span></span>

<span data-ttu-id="261af-514">Od března 10 2021 jsme s radostí oznamujeme dostupnost **nového prostředí pro obchodování v CSP pro Azure v Rusku**.</span><span class="sxs-lookup"><span data-stu-id="261af-514">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="261af-515">Toto prostředí zjednodušuje a vylepšuje způsob, jakým zákazníci kupují a využívají služby Azure.</span><span class="sxs-lookup"><span data-stu-id="261af-515">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="261af-516">Poskytne také partnerům v programu CSP konzistentní pohled na ceny Azure napříč prodejními pohyby, ceny za USD pro globální konzistenci, zarovnání data fakturace a přístup k Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="261af-516">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="261af-517">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-517">Next steps</span></span>

<span data-ttu-id="261af-518">K dispozici je několik prostředků, které představují nové prostředí Azure Commerce a poskytují další informace.</span><span class="sxs-lookup"><span data-stu-id="261af-518">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="261af-519">Nejnovější Nejčastější dotazy, balíčky, video a další informace najdete v [galerii prostředků aktualizace programu CSP](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span><span class="sxs-lookup"><span data-stu-id="261af-519">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="261af-520">Licenční klíč softwaru partnerského centra a stažení</span><span class="sxs-lookup"><span data-stu-id="261af-520">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="261af-521">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-521">Categories</span></span>

- <span data-ttu-id="261af-522">Datum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="261af-522">Date: 2021-03-04</span></span>
- <span data-ttu-id="261af-523">Možnosti</span><span class="sxs-lookup"><span data-stu-id="261af-523">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="261af-524">Souhrn</span><span class="sxs-lookup"><span data-stu-id="261af-524">Summary</span></span>

<span data-ttu-id="261af-525">Funkce pro stažení softwaru partnerského centra a plnění licenčního klíče se znovu nainstalovala.</span><span class="sxs-lookup"><span data-stu-id="261af-525">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-526">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-526">Impacted audience</span></span>

<span data-ttu-id="261af-527">Všichni partneři poskytovatele Cloud Solution Provider (CSP) postupující trvalé a serverové objednávky softwaru prostřednictvím partnerského centra</span><span class="sxs-lookup"><span data-stu-id="261af-527">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="261af-528">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-528">Details</span></span>

<span data-ttu-id="261af-529">V reakci na zpětnou vazbu od partnerů aktualizujeme možnost plnění partnerského centra a získáte software a licenční klíče pro trvalé objednávky softwaru a předplatného serveru.</span><span class="sxs-lookup"><span data-stu-id="261af-529">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="261af-530">Před odstraněním 19. ledna 2021 se obnoví do předchozího stavu.</span><span class="sxs-lookup"><span data-stu-id="261af-530">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="261af-531">(Viz [oznámení](2020-september.md#17).)</span><span class="sxs-lookup"><span data-stu-id="261af-531">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="261af-532">Všimněte si, že licenční klíče softwaru a odkazy ke stažení jsou cenné a vysoce vyhledané – po prostředcích duševního vlastnictví.</span><span class="sxs-lookup"><span data-stu-id="261af-532">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="261af-533">Pokud dojde k úniku, můžou se rychle vyčerpat z jejich aktivačních limitů a způsobit negativní činnost zákazníků a partnerů.</span><span class="sxs-lookup"><span data-stu-id="261af-533">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="261af-534">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-534">Next steps</span></span>

<span data-ttu-id="261af-535">Pokyny k používání a důležité pokyny k distribuci softwarového klíče najdete v následujících zdrojích informací:</span><span class="sxs-lookup"><span data-stu-id="261af-535">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="261af-536">Prodej místního softwaru prostřednictvím programu CSP</span><span class="sxs-lookup"><span data-stu-id="261af-536">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="261af-537">[Průvodce vytvořením nové obchodní příručky pro partnerský](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) software (viz část **pokyny k distribuci softwarových klíčů** )</span><span class="sxs-lookup"><span data-stu-id="261af-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="261af-538">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="261af-538">Questions?</span></span>

<span data-ttu-id="261af-539">Pokud máte další dotazy k tomuto oznámení, Projděte si příslušné komunity Yammeru.</span><span class="sxs-lookup"><span data-stu-id="261af-539">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="261af-540">Migrace vašich obchodů z partnera Sales Connect (PSC) do partnerského centra</span><span class="sxs-lookup"><span data-stu-id="261af-540">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="261af-541">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-541">Categories</span></span>

- <span data-ttu-id="261af-542">Datum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="261af-542">Date: 2021-03-04</span></span>
- <span data-ttu-id="261af-543">Možnosti</span><span class="sxs-lookup"><span data-stu-id="261af-543">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="261af-544">Souhrn</span><span class="sxs-lookup"><span data-stu-id="261af-544">Summary</span></span>

<span data-ttu-id="261af-545">Partner Sales Connect (PSC) se přesune k přístupu jen pro čtení od 31. března 2021, proto doporučujeme začít migrovat vaše obchody z PSC do partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="261af-545">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-546">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-546">Impacted audience</span></span>

<span data-ttu-id="261af-547">Partneři s obchody v PBV</span><span class="sxs-lookup"><span data-stu-id="261af-547">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="261af-548">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-548">Details</span></span>

<span data-ttu-id="261af-549">V rámci našeho sdíleného závazku na růst se dá **společně prodávat pomocí Microsoftu** cesta, která se má **zjistit, zajistit vaše odbornost a rozšířit nároky zákazníků** na pozitivní výsledky zákazníků.</span><span class="sxs-lookup"><span data-stu-id="261af-549">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="261af-550">Díky průměrnému obchodování, který je **3,5 časů rychleji** než normální, vám Správa možností společného prodeje v partnerském centru umožní prodávat přes přímé kanály zákazníka, partnera a prodejce Microsoftu a spravovat celý kanál odkazů na jednom místě.</span><span class="sxs-lookup"><span data-stu-id="261af-550">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="261af-551">**PBV** se přesune k **přístupu jen pro čtení** od **31. března 2021**, proto doporučujeme začít přesun do partnerského centra a získat přístup k těmto vylepšením schopností:</span><span class="sxs-lookup"><span data-stu-id="261af-551">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="261af-552">Přesnější **Směrování** všech obchodů, které sdílíte s Microsoftem, s dopravou prodávající na základě typu pomoci, kterou potřebujete.</span><span class="sxs-lookup"><span data-stu-id="261af-552">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="261af-553">**Ověření nároku** na zajištění opravňujícího řešení pro pobídku a pro splnění kritérií programu ISV Connect, které zjednodušují proces schvalování a konečné ověření platnosti (PoE).</span><span class="sxs-lookup"><span data-stu-id="261af-553">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="261af-554">**Bezproblémové uživatelské prostředí** pro správu všech příležitostí společného prodeje a potenciálních zákazníků na jednom místě.</span><span class="sxs-lookup"><span data-stu-id="261af-554">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="261af-555">V partnerském centru jsme také nedávno přidali nové funkce, které vám pomůžou při přesunu:</span><span class="sxs-lookup"><span data-stu-id="261af-555">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="261af-556">Hromadné operace pro společný prodej příležitostí</span><span class="sxs-lookup"><span data-stu-id="261af-556">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="261af-557">[Funkce migrace koupě](../psc-to-pc.md) (viz část věnované **migraci PSC** .)</span><span class="sxs-lookup"><span data-stu-id="261af-557">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="261af-558">S využitím možností společného prodeje v partnerském centru budou mít prodejní týmy víc času na zaměření na Nurturing potenciálních zákazníků a příležitostí, uzavírání obchodů a vytváření trvalých vztahů se zákazníky.</span><span class="sxs-lookup"><span data-stu-id="261af-558">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="261af-559">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-559">Next steps</span></span>

<span data-ttu-id="261af-560">Pomocí [Průvodce přechodem](../psc-to-pc.md) k partnerským centrům vás seznámíte s postupem migrace vašich obchodů z PSC do partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="261af-560">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="261af-561">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="261af-561">Questions?</span></span>

<span data-ttu-id="261af-562">Pokud chcete mít další otázky, obraťte se na [podporu](https://partner.microsoft.com/support/?stage=1).</span><span class="sxs-lookup"><span data-stu-id="261af-562">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="261af-563">Nové produkty a nabídky společnosti Microsoft Dynamics 365, které jsou k dispozici od 1. dubna 2021</span><span class="sxs-lookup"><span data-stu-id="261af-563">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="261af-564">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-564">Categories</span></span>

- <span data-ttu-id="261af-565">Datum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="261af-565">Date: 2021-03-04</span></span>
- <span data-ttu-id="261af-566">Možnosti</span><span class="sxs-lookup"><span data-stu-id="261af-566">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="261af-567">Souhrn</span><span class="sxs-lookup"><span data-stu-id="261af-567">Summary</span></span>

<span data-ttu-id="261af-568">Od 1. dubna 2021 bude Microsoft spouštět několik nových produktů a nabídek pro program poskytovatele Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="261af-568">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-569">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-569">Impacted audience</span></span>

<span data-ttu-id="261af-570">Všechny partnery, kteří se docházejí prostřednictvím programu Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="261af-570">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="261af-571">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-571">Details</span></span>

<span data-ttu-id="261af-572">Od 1. dubna 2021 bude Microsoft spouštět následující nové produkty a nabídky:</span><span class="sxs-lookup"><span data-stu-id="261af-572">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="261af-573">Power BI Premium na uživatele</span><span class="sxs-lookup"><span data-stu-id="261af-573">Power BI Premium Per User</span></span>
- <span data-ttu-id="261af-574">USL a rozšiřování geografických a segmentů zákazníků</span><span class="sxs-lookup"><span data-stu-id="261af-574">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="261af-575">**Power BI Premium na uživatele**</span><span class="sxs-lookup"><span data-stu-id="261af-575">**Power BI Premium Per User**</span></span>

<span data-ttu-id="261af-576">Microsoft bude zavádět první nabídky Power BI Premium pro jednotlivé uživatele.</span><span class="sxs-lookup"><span data-stu-id="261af-576">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="261af-577">Power BI Premium se aktuálně prodává pouze v konstrukci kapacity.</span><span class="sxs-lookup"><span data-stu-id="261af-577">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="261af-578">Power BI Premium pro jednotlivé uživatele poskytuje přístup k funkcím Enterprise business intelligence (BI) a Analytics.</span><span class="sxs-lookup"><span data-stu-id="261af-578">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="261af-579">Flexibilní organizace pro licencování jednotlivých stanic na malé a střední firmy.</span><span class="sxs-lookup"><span data-stu-id="261af-579">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="261af-580">Další informace o této nabídce najdete v [podrobnostech o verzi Power BI](/power-platform-release-plan/2020wave2/power-bi/planned-features) .</span><span class="sxs-lookup"><span data-stu-id="261af-580">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="261af-581">**Podrobnosti nabídky**</span><span class="sxs-lookup"><span data-stu-id="261af-581">**Offer details**</span></span>

<span data-ttu-id="261af-582">Všimněte si, že název nabídky se mírně liší od ceníku ve verzi Preview.</span><span class="sxs-lookup"><span data-stu-id="261af-582">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="261af-583">Název nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-583">Offer name</span></span> | <span data-ttu-id="261af-584">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-584">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="261af-585">Power BI Premium na uživatele</span><span class="sxs-lookup"><span data-stu-id="261af-585">Power BI Premium Per User</span></span> | <span data-ttu-id="261af-586">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="261af-586">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="261af-587">Power BI Premium na uživatele pro vyučujícího</span><span class="sxs-lookup"><span data-stu-id="261af-587">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="261af-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="261af-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="261af-589">Power BI Premium na uživatele pro studenty</span><span class="sxs-lookup"><span data-stu-id="261af-589">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="261af-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="261af-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="261af-591">Power BI Premium na uživatele (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="261af-591">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="261af-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="261af-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="261af-593">Power BI Premium pro uživatele Add-On</span><span class="sxs-lookup"><span data-stu-id="261af-593">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="261af-594">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="261af-594">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="261af-595">Power BI Premium Add-On na uživatele pro vyučující</span><span class="sxs-lookup"><span data-stu-id="261af-595">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="261af-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="261af-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="261af-597">Power BI Premium Add-On na uživatele pro studenty</span><span class="sxs-lookup"><span data-stu-id="261af-597">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="261af-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="261af-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="261af-599">Power BI Premium Add-On na uživatele (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="261af-599">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="261af-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="261af-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="261af-601">**USL a rozšiřování geografických a segmentů zákazníků**</span><span class="sxs-lookup"><span data-stu-id="261af-601">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="261af-602">Jako při spuštění z prosince 2020 se přidávají nabídky hlasu a marketingu pro zákazníky Dynamics 365 za účelem přidání nových zemí a dalších neziskových a vzdělávacích SKU.</span><span class="sxs-lookup"><span data-stu-id="261af-602">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="261af-603">Název nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-603">Offer name</span></span> | <span data-ttu-id="261af-604">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-604">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="261af-605">Dynamics 365 Customer Voice USL (ceny neziskových zaměstnanců)</span><span class="sxs-lookup"><span data-stu-id="261af-605">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="261af-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="261af-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="261af-607">Dynamics 365 Customer Voice USL pro vyučujícího</span><span class="sxs-lookup"><span data-stu-id="261af-607">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="261af-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="261af-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="261af-609">Další informace o těchto nabídkách najdete na následujících stránkách:</span><span class="sxs-lookup"><span data-stu-id="261af-609">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="261af-610">Domovská stránka hlasu pro zákaznickou službu Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="261af-610">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="261af-611">Domovská stránka marketingu Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="261af-611">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="261af-612">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-612">Next steps</span></span>

<span data-ttu-id="261af-613">Projděte si materiály k tomuto tématu a sdílejte tyto informace s příslušnými zúčastněnými stranami ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="261af-613">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="261af-614">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="261af-614">Questions?</span></span>

<span data-ttu-id="261af-615">Jakékoli otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.</span><span class="sxs-lookup"><span data-stu-id="261af-615">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="261af-616">Univerzální tisk společnosti Microsoft je nyní k dispozici v některých sadách.</span><span class="sxs-lookup"><span data-stu-id="261af-616">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="261af-617">Kategorie</span><span class="sxs-lookup"><span data-stu-id="261af-617">Categories</span></span>

- <span data-ttu-id="261af-618">Datum: 2021-03-33</span><span class="sxs-lookup"><span data-stu-id="261af-618">Date: 2021-03-33</span></span>
- <span data-ttu-id="261af-619">Možnosti</span><span class="sxs-lookup"><span data-stu-id="261af-619">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="261af-620">Souhrn</span><span class="sxs-lookup"><span data-stu-id="261af-620">Summary</span></span>

<span data-ttu-id="261af-621">Univerzální tisk společnosti Microsoft bude k dispozici pro transakce v rámci vybraných Microsoft 365ch sad a jako samostatný doplněk od 1. března 2021.</span><span class="sxs-lookup"><span data-stu-id="261af-621">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="261af-622">Ovlivněná cílová skupina</span><span class="sxs-lookup"><span data-stu-id="261af-622">Impacted audience</span></span>

<span data-ttu-id="261af-623">Všechny partnery, kteří se docházejí prostřednictvím programu Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="261af-623">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="261af-624">Podrobnosti</span><span class="sxs-lookup"><span data-stu-id="261af-624">Details</span></span>

<span data-ttu-id="261af-625">[Univerzální tisk](https://aka.ms/universalprint) je Microsoft 365 tisková služba, která odstraňuje potřebu místních tiskových serverů a umožňuje zařízením s Windows tisk na tiskárnách registrovaných v Azure.</span><span class="sxs-lookup"><span data-stu-id="261af-625">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="261af-626">Bude k dispozici pro Transact od 1. března 2021.</span><span class="sxs-lookup"><span data-stu-id="261af-626">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="261af-627">Pracovní procesy využívají tisk bez ovladačů, zjednodušené zjišťování tiskáren založené na poloze a intuitivní možnosti tisku bez výukové křivky.</span><span class="sxs-lookup"><span data-stu-id="261af-627">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="261af-628">Zařízení, která jsou připojená k Azure Active Directory (Azure AD), používají k bezpečnému tisku existující přihlašovací údaje Azure AD.</span><span class="sxs-lookup"><span data-stu-id="261af-628">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="261af-629">Správci spravují tisk pomocí Azure Portal a můžou snadno připojit tiskárny s nativní podporou univerzálního tisku.</span><span class="sxs-lookup"><span data-stu-id="261af-629">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="261af-630">Univerzální tisk se dá nasadit s nekompatibilními tiskárnami pomocí softwaru univerzálního tiskového konektoru.</span><span class="sxs-lookup"><span data-stu-id="261af-630">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="261af-631">Univerzální tisk bude při spuštění vyplněn ve Windows E3, a3, E5 a A5 a Microsoft 365 BP, F3, E3, a3, E5 a a5.</span><span class="sxs-lookup"><span data-stu-id="261af-631">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="261af-632">**Podrobnosti nabídky**</span><span class="sxs-lookup"><span data-stu-id="261af-632">**Offer details**</span></span>

<span data-ttu-id="261af-633">Všimněte si, že název nabídky se mírně liší od ceníku ve verzi Preview.</span><span class="sxs-lookup"><span data-stu-id="261af-633">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="261af-634">Název nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-634">Offer name</span></span> | <span data-ttu-id="261af-635">ID nabídky</span><span class="sxs-lookup"><span data-stu-id="261af-635">Offer ID</span></span> | <span data-ttu-id="261af-636">ID materiálu</span><span class="sxs-lookup"><span data-stu-id="261af-636">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="261af-637">Doplněk objemu univerzálního tisku (úlohy 500) – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="261af-637">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="261af-638">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="261af-638">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="261af-639">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="261af-639">9BI-00004</span></span>   |
| <span data-ttu-id="261af-640">Doplněk objemu univerzálního tisku (úlohy 500) pro vyučující – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="261af-640">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="261af-641">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="261af-641">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="261af-642">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="261af-642">9BK-00004</span></span>   |
| <span data-ttu-id="261af-643">Doplněk objemu univerzálního tisku (úlohy 500) – Windows</span><span class="sxs-lookup"><span data-stu-id="261af-643">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="261af-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="261af-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="261af-645">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="261af-645">9BI-00002</span></span>   |
| <span data-ttu-id="261af-646">Doplněk objemu univerzálního tisku (úlohy 500) pro vyučujícího – Windows</span><span class="sxs-lookup"><span data-stu-id="261af-646">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="261af-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="261af-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="261af-648">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="261af-648">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="261af-649">Další kroky</span><span class="sxs-lookup"><span data-stu-id="261af-649">Next steps</span></span>

<span data-ttu-id="261af-650">Seznamte se s ceníkem a s [přehledem univerzálního tisku](/universal-print/fundamentals/universal-print-whatis).</span><span class="sxs-lookup"><span data-stu-id="261af-650">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="261af-651">Tyto informace Sdílejte se všemi odpovídajícími kontakty ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="261af-651">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="261af-652">Máte otázky?</span><span class="sxs-lookup"><span data-stu-id="261af-652">Questions?</span></span>

<span data-ttu-id="261af-653">Jakékoli otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.</span><span class="sxs-lookup"><span data-stu-id="261af-653">For any questions about these offers, check your relevant Yammer communities.</span></span>
